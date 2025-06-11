<template>
    <HomeBackground class="gap-12">

        <div class="italic text-8xl font-bold drop-shadow-lg/90 ">

            <div class="animate-move-in"
            style="--tw-move-x: -50px; --tw-move-time: 1s;">

                <span class="text-gray-200">
                    FROM
                </span>

                <span class="bg-gradient-to-br from-sky-500
                to-violet-500 to-80% bg-clip-text
                text-transparent pr-2">
                    BEGINNING
                </span>
                
            </div>

            <div class="ml-31 animate-move-in"
            style="--tw-move-x: 50px; --tw-move-time: 1s;">

                <span class="text-gray-200">
                    TO
                </span>

                <span class="bg-gradient-to-br from-red-500
                to-pink-500 to-80% bg-clip-text
                text-transparent pr-2">
                    BEAST
                </span>

            </div>

        </div>

        <div class="animate-move-in font-bold flex flex-col items-center
        gap-10"
        style="--tw-move-time: 1s;">

            <span class="text-4xl text-gray-200 text-shadow-lg/80">
                We’ve Got You Covered
            </span>
            
            <div class="bg-black/30 p-3 backdrop-blur-xl rounded-md">
                <a href="#" class="gradient-text text-transparent
                font-bold text-2xl p-1">START NOW</a>
            </div>

        </div>

    </HomeBackground>
</template>

<script setup>
    import HomeBackground from '@/components/HomeBackground.vue';
</script>