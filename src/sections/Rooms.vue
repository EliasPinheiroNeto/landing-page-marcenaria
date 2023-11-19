<script setup lang="ts">
import { onMounted, reactive } from 'vue';

import CarouselImages from '@/components/CarouselImages.vue';

const slide = reactive({
    position: 0,
    step: 1,
    resources: [
        "https://placehold.co/600x400?text=1",
        "https://placehold.co/600x400?text=2",
        "https://placehold.co/600x400?text=3",
        "https://placehold.co/600x400?text=4",
        "https://placehold.co/600x400?text=5"
    ]
})

onMounted(() => {
    if (innerWidth >= 640) {
        slide.step = 0.5
    }
})

function next() {
    if (slide.position >= (slide.resources.length * slide.step) - 1) {
        slide.position = 0
    } else {
        slide.position += slide.step
    }
}

function prev() {
    if (slide.position <= 0) {
        slide.position = slide.resources.length - 1
    } else {
        slide.position -= slide.step
    }
}
</script> 

<template>
    <div class="border-orange-50">
        <section class="container mx-auto
        p-4 ">
            <h2 class="text-center
            text-2xl mb-2
            md:text-4xl md:mb-4">Quartos</h2>

            <!-- Carousel -->
            <div class="overflow-x-hidden relative">
                <div class="flex transition-transform"
                     :style="{ transform: `translateX(-${slide.position * 100}%)` }">

                    <CarouselImages v-for="i in slide.resources"
                                    :src="i" />

                </div>

                <!-- Buttons -->
                <div class="absolute inset-0 flex justify-between 
                px-4
                sm:px-2">
                    <button @click="prev()">
                        <img class="rotate-180
                        h-6
                        sm:h-8"
                             src="../assets/maior_que.png"
                             alt="">
                    </button>

                    <button @click="next()">
                        <img class="
                        h-6
                        sm:h-8"
                             src="../assets/maior_que.png"
                             alt="">
                    </button>
                </div>
            </div>

        </section>
    </div>
</template> 

<style scoped></style> 
