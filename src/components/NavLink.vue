<template>
  <a :href="to" class="hover:text-transparent hover:scale-120
  hover:text-shadow-lg/20 hover:text-shadow-purple-400 gradient-text
  transition-all duration-200 text-gray-200 font-semibold
  text-shadow-md/70 active:animate-none">
    <slot></slot>
  </a>
</template>

<script setup>
  defineProps({
    to: {
      type: String,
      required: true
    }
  });
</script>