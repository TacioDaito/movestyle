<template>
    <HomeBackground>

        <h1
            class="gap-1 mt-6 sm:mt-14 italic text-5xl sm:text-6xl md:text-7xl lg:text-8xl font-bold drop-shadow-lg/90 flex flex-col items-center">
            <div class="gap-x-2 animate-move-in flex flex-col sm:flex-row items-center"
                style="--tw-move-x: -50px; --tw-move-time: 1s;">
                <span class="text-gray-200">FROM</span>
                <span class="px-2 bg-gradient-to-br from-sky-500 to-violet-500 to-80% bg-clip-text text-transparent">
                    BEGINNING
                </span>
            </div>

            <div class="gap-x-2 animate-move-in flex flex-col sm:flex-row items-center"
                style="--tw-move-x: 50px; --tw-move-time: 1s;">
                <span class="text-gray-200">TO</span>
                <span class="px-2 bg-gradient-to-br from-red-500 to-pink-500 to-80% bg-clip-text text-transparent">
                    BEAST
                </span>
            </div>
        </h1>

        <h2 class="text-xl sm:text-2xl md:text-3xl lg:text-4xl font-bold text-gray-200 text-shadow-lg/40 text-center animate-move-in"
            style="--tw-move-time: 1s;">
            We’ve Got You Covered
        </h2>

        <div class="p-1 bg-black/50 backdrop-blur-md rounded-md flex justify-center animate-move-in"
            style="--tw-move-time: 1s;">
            <a href="#" class="p-1 font-bold text-lg sm:text-xl md:text-2xl lg:text-3xl gradient-text text-transparent">
                START NOW
            </a>
        </div>

    </HomeBackground>
</template>

<script setup>
import HomeBackground from '@/components/HomeBackground.vue';
</script>