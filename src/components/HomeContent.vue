<template>
    <HomeBackground>

        <div class="italic text-8xl font-bold mt-4 drop-shadow-lg/90">
            <div class="animate-move-in animate-move-in-from-left"
            style="--tw-move-x: -50px; --tw-move-time: 1s;">
                <span class="text-gray-200
                text-shadow-lg/80">
                    FROM
                </span>
                <span class="bg-gradient-to-br
                from-sky-500 to-violet-500 to-80% inline-block
                bg-clip-text text-transparent">
                    BEGINNING
                </span>
            </div>
            <div class="ml-31 animate-move-in animate-move-in-from-right"
            style="--tw-move-x: 50px; --tw-move-time: 1s;">
                <span class="text-gray-200">
                    TO
                </span>
                <span class="bg-gradient-to-br
                from-red-500 to-pink-500 to-80% w-90 inline-block
                bg-clip-text text-transparent">
                    BEAST
                </span>
            </div>
        </div>
        <div class="animate-move-in" style="--tw-move-time: 1s;">
            <div class="flex justify-center mt-8">
                <span class="text-4xl text-gray-200 font-bold
                text-shadow-lg/80">
                    We’ve Got You Covered
                </span>
            </div>
            <div class="flex justify-center">
                <div class="mt-10 rounded-sm
                bg-black/30 backdrop-blur-md flex
                items-center justify-center">
                    <a href="#" class="gradient-text text-transparent
                    font-bold text-2xl py-2 px-3">START NOW</a>
                </div>
            </div>
        </div>

    </HomeBackground>
</template>

<script setup>
    import HomeBackground from '@/components/HomeBackground.vue';
</script>