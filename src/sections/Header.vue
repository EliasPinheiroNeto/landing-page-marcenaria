<script setup lang="ts"></script> 

<template>
    <div class="w-full bg-blue-500">
        <header class="container h-full mx-auto flex py-2
        flex-col px-4
        sm:flex-row sm:justify-between sm:items-center sm:px-12">

            <a class="mb-4 h-1 flex-grow w-2/3 mx-auto
            sm:mb-0 sm:h-full sm:flex-grow-0 sm:w-auto sm:mx-0"
               href="/">
                <img class="object-cover 
                h-full w-full"
                     src="https://placehold.co/800x400?text=Logo"
                     alt="Site Logo">
            </a>
            <nav>
                <ul class="flex text-white text-lg
            justify-between
            sm:gap-x-8">
                    <li>
                        <a href="#about">Quem somos?</a>
                    </li>
                    <li>
                        <a href="#gallery">Galeria</a>
                    </li>
                    <li>
                        <a href="#email">Fale Conosco</a>
                    </li>
                </ul>
            </nav>
        </header>
    </div>
</template> 

<style scoped></style> 
