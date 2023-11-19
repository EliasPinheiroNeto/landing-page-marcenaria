<script setup lang="ts"></script> 

<template>
    <div class="bg-blue-500">
        <section class="h-full mx-auto
        flex flex-col-reverse
        sm:grid sm:grid-cols-5
        md:sm:grid-cols-7
        2xl:container 2xl:mx-auto">
            <div class="
            flex-grow
            sm:col-span-3 sm:h-auto
            md:col-span-4">
                <img class="block h-full object-cover"
                     src="https://placehold.co/400?text=Banner"
                     alt="">
            </div>

            <div class="grid text-white
            px-4 py-12 grid-cols-1
            sm:grid-rows-2 sm:h-auto sm:px-8 sm:py-16">
                <!-- Texto forte -->
                <div class="
                mx-auto
                sm:mx-0">
                    <h1 class="text-6xl">Transforme <br>
                        <span class="text-3xl">a sua <strong>casa</strong></span>
                    </h1>
                </div>
                <!-- Texto fraco -->
                <div class="
                hidden
                sm:flex items-center">
                    <a class="text-xl"
                       href="#">- Fale Conosco</a>
                </div>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 
