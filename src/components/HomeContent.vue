<template>
    <HomeBackground class="gap-8 md:gap-14">

        <div
            class="mt-4 md:mt-14 gap-2 italic text-5xl md:text-6xl lg:text-8xl font-bold drop-shadow-lg/90 flex flex-col items-center"
        >
            <div
                class="gap-2 animate-move-in flex flex-col md:flex-row items-center"
                style="--tw-move-x: -50px; --tw-move-time: 1s;"
            >
                <span class="text-gray-200">FROM</span>
                <span
                    class="px-2 bg-gradient-to-br from-sky-500 to-violet-500 to-80% bg-clip-text text-transparent"
                >
                    BEGINNING
                </span>
            </div>

            <div
                class="gap-2 animate-move-in flex flex-col md:flex-row items-center"
                style="--tw-move-x: 50px; --tw-move-time: 1s;"
            >
                <span class="text-gray-200">TO</span>
                <span
                    class="px-2 bg-gradient-to-br from-red-500 to-pink-500 to-80% bg-clip-text text-transparent"
                >
                    BEAST
                </span>
            </div>
        </div>

        <div
            class="gap-8 md:gap-14 animate-move-in font-bold flex flex-col items-center"
            style="--tw-move-time: 1s;"
        >
            <span
                class="text-2xl md:text-3xl lg:text-4xl text-gray-200 text-shadow-lg/40 text-center"
            >
                We’ve Got You Covered
            </span>

            <div class="p-2 bg-black/50 backdrop-blur-md rounded-md">
                <a
                    href="#"
                    class="p-1 font-bold text-lg md:text-xl lg:text-2xl gradient-text text-transparent"
                >
                    START NOW
                </a>
            </div>

        </div>
    </HomeBackground>
</template>

<script setup>
    import HomeBackground from '@/components/HomeBackground.vue';
</script>