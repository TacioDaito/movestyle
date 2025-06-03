<template>
  <div id="navbar" class="fixed top-0 left-1/2 transform -translate-x-1/2 z-50 w-160
  transition-[background] duration-300 text-lg
  [clip-path:polygon(0%_0%,100%_0%,95%_100%,5%_100%)] flex justify-center">
    <div class="flex justify-evenly items-center w-9/10">
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
  window.addEventListener('scroll', () => {
    const navbar = document.getElementById('navbar');
    navbar.classList.toggle('bg-black/50', window.scrollY > 10);
  });
</script>