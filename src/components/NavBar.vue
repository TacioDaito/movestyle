<template>
  <div class="navbar fixed top-0 left-1/2 transform -translate-x-1/2 z-50 w-170
              transition-[background] duration-300 text-lg
              [clip-path:polygon(0%_0%,100%_0%,88%_100%,12%_100%)] flex justify-center
              bg-black/30
              bg-[repeating-linear-gradient(45deg,_transparent,_transparent_4px,_rgba(60,60,60,0.3)_4px,_rgba(60,60,60,0.3)_5px),repeating-linear-gradient(-45deg,_transparent,_transparent_200px,_rgba(40,40,40,0.3)_200px,_rgba(40,40,40,0.3)_201px)]
              backdrop-blur-sm">
    <div class="flex justify-evenly items-center w-9/10">
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
  // import { onMounted, onUnmounted } from 'vue';

  // const handleScroll = () => {
  //   const navbar = document.querySelector('.navbar');
  //   navbar.classList.toggle('bg-black/30', window.scrollY > 10);
  //   navbar.classList.toggle('bg-[repeating-linear-gradient(45deg,_transparent,_transparent_10px,_rgba(128,128,128,0.3)_10px,_rgba(128,128,128,0.3)_11px,_transparent_12px,_transparent_50px)]', window.scrollY > 50);
  // };

  // onMounted(() => {
  // window.addEventListener('scroll', handleScroll);
  // });

  // onUnmounted(() => {
  // window.removeEventListener('scroll', handleScroll);
  // });
</script>