<template>
  <div class="fixed top-2 left-1/2 transform -translate-x-1/2 z-50
  flex items-center justify-evenly min-w-xl animate-move-in
  dashed-div" style="--tw-move-y: -10px;"
  >
    <NavRow>
      <NavLink to="#">HOME</NavLink>
      <NavLink to="#">PLANS</NavLink>
    </NavRow>
    <LogoImage/>
    <NavRow>
      <NavLink to="#">CLASSES</NavLink>
      <NavLink to="#">CONTACT</NavLink>
    </NavRow>
  </div>
</template>

<script setup>
  import NavLink from '@/components/NavLink.vue';
  import NavRow from '@/components/NavRow.vue';
  import LogoImage from '@/components/LogoImage.vue';
</script>