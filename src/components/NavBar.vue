<template>

  <div class="hidden md:flex fixed top-4 left-1/2 transform -translate-x-1/2 z-10
  items-center justify-evenly w-xl h-12 animate-move-in
  dashed-div " style="--tw-move-y: -10px;">
    <LogoImage />
    <NavLink to="#">HOME</NavLink>
    <NavLink to="#">PLANS</NavLink>
    <NavLink to="#"></NavLink>
    <NavLink to="#">CLASSES</NavLink>
    <NavLink to="#">CONTACT</NavLink>
  </div>

  <label class="group">
    <input type="checkbox" class="peer hidden" />
    <div class="md:hidden flex fixed top-4 left-1/2 transform -translate-x-1/2 z-10
    justify-evenly w-30 h-20 animate-move-in transition-all duration-200
    dashed-div peer-checked:h-68" style="--tw-move-y: -10px;">
      <LogoImage />
      <div class="relative w-9 h-3 top-15 bg-white opacity-30 [clip-path:polygon(0%_0%,100%_0%,50%_100%)]
        group-has-[:checked]:[clip-path:polygon(50%_0%,100%_100%,0%_100%)]">
      </div>
      <div class="opacity-0 group-has-[:checked]:opacity-100 absolute top-22 space-y-3 transition-all duration-200">
        <NavLink to="#">HOME</NavLink>
        <NavLink to="#">PLANS</NavLink>
        <NavLink to="#">CLASSES</NavLink>
        <NavLink to="#">CONTACT</NavLink>
      </div>
    </div>
  </label>

</template>

<script setup>
import NavLink from '@/components/NavLink.vue';
import LogoImage from '@/components/LogoImage.vue';
</script>