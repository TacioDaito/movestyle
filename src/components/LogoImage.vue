<template>
    <img src="@/assets/images/movestyle.svg" alt="Icon"
    class="logo w-20 h-20 mx-4 drop-shadow-md/70 transition-filter duration-300"/>
</template>

<script setup>

import { onMounted, onUnmounted } from 'vue';

    const handleScroll = () => {
        const logos = document.querySelectorAll('.logo');
        logos.forEach(logo => {
            logo.classList.toggle('drop-shadow-md/70', window.scrollY < 10);
        });
    };

    onMounted(() => {
    window.addEventListener('scroll', handleScroll);
    });

    onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
    });

</script>