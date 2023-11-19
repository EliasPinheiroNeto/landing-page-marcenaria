<script setup lang="ts"></script> 

<template>
    <div class="bg-blue-500">
        <section class="h-full mx-auto
        flex flex-col-reverse
        sm:grid sm:grid-cols-5
        2xl:container 2xl:mx-auto">
            <div class="
            h-full flex flex-col
            sm:col-span-2 sm:h-auto sm:flex-grow-0">
                <img class="object-cover h-1 flex-grow"
                     src="https://placehold.co/400?text=Banner"
                     alt="">
            </div>

            <!-- Textos -->
            <div class="grid text-white
            px-4 py-12 grid-cols-1
            sm:grid-rows-2 sm:h-auto sm:px-8 sm:py-16 sm:col-span-3">
                <div class="
                mx-auto
                sm:mx-0">
                    <h1 class="text-6xl">Transforme <br>
                        <span class="text-3xl">a sua <strong>casa</strong></span>
                    </h1>
                </div>

                <div class="
                hidden
                sm:flex items-center">
                    <a class="text-xl"
                       href="#about">- Fale Conosco</a>
                </div>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 
