<template>
  <a :href="to" class="navlink hover:text-transparent hover:scale-120
  hover:text-shadow-md/20 hover:text-shadow-purple-300 bg-clip-text
  bg-gradient-to-r from-sky-300 via-purple-300 to-pink-300 transition-all
  duration-200 text-gray-200 font-medium text-shadow-md/70">
    <slot></slot>
  </a>
</template>

<script setup>
import { onMounted, onUnmounted } from 'vue';

  defineProps({
    to: {
      type: String,
      required: true
    }
  });

  const handleScroll = () => {
    const navlinks = document.querySelectorAll('.navlink');
    navlinks.forEach(navlink => {
        navlink.classList.toggle('text-shadow-md/70', window.scrollY < 10);
    });
  };

  onMounted(() => {
  window.addEventListener('scroll', handleScroll);
  });

  onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
  });

</script>