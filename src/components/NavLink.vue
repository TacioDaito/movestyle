<template>
  <a :href="to" class="navlink hover:text-transparent hover:scale-120
  hover:text-shadow-lg/20 hover:text-shadow-purple-400 bg-clip-text
  bg-linear-[90deg,#8ff8ff,#a58fff_16%,#ff8fd8_33%,#a58fff_49%,#8ff8ff_66%,#a58fff_82%,#ff8fd8]
  bg-repeat-x bg-[length:300%_auto] animate-gradient transition-all
  duration-200 text-gray-200 font-medium text-shadow-md/70
  active:animate-none">
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