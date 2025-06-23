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
    <div ref="plansDiv"
         style="--tw-move-time: 1s; --tw-move-y: -50px;">
        <div class="flex flex-col items-center justify-center relative h-screen bg-gray-900 text-white">
            <h1 class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl font-bold mb-4 animate-move-in"
                style="--tw-move-time: 1s;">
            PLANS
            </h1>
            <p class="text-xl sm:text-2xl md:text-3xl lg:text-4xl mb-8 animate-move-in"
                style="--tw-move-time: 1s;">
            Choose the plan that suits you best
            </p>
            <div class="p-4 bg-black/50 backdrop-blur-md rounded-md animate-move-in"
                 style="--tw-move-time: 1s;">
            <a href="#" class="text-lg sm:text-xl md:text-2xl lg:text-3xl font-bold gradient-text text-transparent">
                GET STARTED
            </a>
            </div>
        </div>
    </div>
</template>