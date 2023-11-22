<script setup lang='ts'>
import { onMounted, onUnmounted, reactive } from 'vue';

const props = defineProps<{
    resources: { src: string, alt?: string }[]
}>()

const carousel = reactive({
    slide: 0,
    show: 1
})
// Arrumar esse componente carrossel

onMounted(() => {
    window.addEventListener("resize", () => {
        if (innerWidth >= 640) {
            carousel.show = 2
        } else {
            carousel.show = 1
        }
    })
})

onUnmounted(() => {
    window.removeEventListener("resize", () => {
        if (innerWidth >= 640) {
            carousel.show = 2
        } else {
            carousel.show = 1
        }
    })
})

function next() {
    if (carousel.slide >= props.resources.length - carousel.show) {
        carousel.slide = 0
    } else {
        carousel.slide++
    }

}

function prev() {
    if (carousel.slide <= 0) {
        carousel.slide = props.resources.length - carousel.show
    } else {
        carousel.slide--
    }
}
</script> 

<template>
    <div class="overflow-x-hidden relative">
        <div class="flex transition-transform"
             :style="{ transform: `translateX(-${carousel.slide * (100 / carousel.show)}%)` }">

            <div class="flex-shrink-0 w-full px-2"
                 :style="{ width: `${100 / carousel.show}%` }"
                 v-for="i in resources">
                <img class="w-full"
                     :src="i.src">
            </div>

        </div>

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
</template> 

<style scoped></style> 
