<script setup>

import { gsap } from 'gsap';
import { onMounted, ref } from 'vue';
import { ScrollTrigger } from 'gsap/ScrollTrigger';
import { ScrollSmoother } from 'gsap/ScrollSmoother';

gsap.registerPlugin(ScrollTrigger, ScrollSmoother);

const plansDiv = ref(null);

onMounted(() => {
  // Div B aparece de baixo e cobre Div A rapidamente
  gsap.from(plansDiv.value, {
    yPercent: 100,
    ease: 'power4.out',
    scrollTrigger: {
      trigger: plansDiv.value,
      start: 'top bottom',
      end: 'top top',
      scrub: 1,
    }
  })
})

const cards = ['Card 1', 'Card 2', 'Card 3']
const active = ref(0)
const prev = () => active.value = (active.value + cards.length - 1) % cards.length
const next = () => active.value = (active.value + 1) % cards.length

</script>

<template>
  <div ref="plansDiv" style="--tw-move-time: 1s; --tw-move-y: -50px;">
    <div class="grid bg-linear-to-bl from-violet-950 to-pink-950 h-screen">
      <div class="col-start-1 row-start-1 bg-yellow-500 h-screen w-screen flex
        items-center justify-center">
      </div>
      <div class="relative col-start-1 row-start-1 w-screen flex flex-col
        items-center justify-center min-h-[60vh] overflow-hidden">
        <!-- Carousel track -->
        <div class="flex transition-transform duration-500 ease-in-out h-160"
          :style="{ transform: `translateX(${33 - (active * 33)}%)` }">
          <div v-for="(card, i) in cards" :key="i"
            class="bg-black/30 w-80 mr-10 rounded-4xl flex items-center justify-center
              text-white text-2xl shrink-0">
            {{ card }}
          </div>
        </div>
        <!-- Arrows -->
        <button @click="prev" class="absolute left-2 top-1/2 -translate-y-1/2
          bg-white/40 rounded-full p-2 z-10">
          &lt;
        </button>
        <button @click="next" class="absolute right-2 top-1/2 -translate-y-1/2
          bg-white/40 rounded-full p-2 z-10">
          &gt;
        </button>
        <!-- Dots -->
        <div class="flex gap-2 mt-6">
          <button v-for="(card, i) in cards" :key="i" @click="active = i"
            :class="['w-3 h-3 rounded-full', active === i ? 'bg-pink-500' : 'bg-white/30']"></button>
        </div>
      </div>
      <!-- <div class="col-start-1 row-start-1 bg-blue-500 h-screen w-screen flex
        items-center justify-center">
        <div class="bg-black/30 rounded-4xl w-xs h-7/10">
        </div>
      </div> -->
      <!-- <div class="col-start-1 row-start-1 bg-red-500 h-screen w-screen flex
        items-center justify-center">
        <div class="bg-black/30 rounded-4xl w-xs h-7/10">
        </div>
      </div> -->
    </div>
  </div>
</template>