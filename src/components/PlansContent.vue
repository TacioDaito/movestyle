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
</script>

<template>
  <div ref="plansDiv" style="--tw-move-time: 1s; --tw-move-y: -50px;">
    <div class="grid bg-linear-to-bl from-violet-950 to-pink-950 h-screen">
      <div class="col-start-1 row-start-1 bg-yellow-500 h-screen w-screen flex items-center justify-center">
        <div class="bg-black/30 rounded-4xl w-xs h-7/10">
        </div>
      </div>
      <!-- <div class="col-start-1 row-start-1 bg-blue-500 h-screen w-screen flex items-center justify-center">
        <div class="bg-black/30 rounded-4xl w-xs h-7/10">
        </div>
      </div> -->
      <!-- <div class="col-start-1 row-start-1 bg-red-500 h-screen w-screen flex items-center justify-center">
        <div class="bg-black/30 rounded-4xl w-xs h-7/10">
        </div>
      </div> -->
    </div>
    <!-- <div class="flex flex-col items-center justify-center relative 
      h-screen bg-linear-to-bl from-violet-950 to-pink-950 text-white">
      <div class="bg-black/30 rounded-4xl w-xs h-7/10">
      </div>
    </div>
    <div class="bg-black h-screen w-screen"></div> -->
  </div>
</template>