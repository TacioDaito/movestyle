<template>
  <a :href="to" class="hover:text-transparent hover:scale-120
  gradient-text transition-transform duration-200
  text-gray-200 font-semibold text-shadow-md/70
  active:animate-none p-1 w-20 text-center block">
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