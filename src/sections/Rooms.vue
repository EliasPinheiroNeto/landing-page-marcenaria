<script setup lang="ts">
import Carousel from '@/components/Carousel.vue';

const resources = [
    {
        src: "https://placehold.co/600x400?text=1"
    },
    {
        src: "https://placehold.co/600x400?text=2"
    },
    {
        src: "https://placehold.co/600x400?text=3"
    },
    {
        src: "https://placehold.co/600x400?text=4"
    },
    {
        src: "https://placehold.co/600x400?text=5"
    },
]
</script> 

<template>
    <div class="border-orange-50">
        <section class="container mx-auto
        p-4 ">
            <h2 class="text-center
            text-2xl mb-2
            md:text-4xl md:mb-4">Quartos</h2>

            <Carousel :resources="resources" />

        </section>
    </div>
</template> 

<style scoped></style> 
