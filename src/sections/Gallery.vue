<script setup lang="ts"></script> 

<template>
     <div class="bg-blue-500"
          id="gallery">
          <section class="container mx-auto grid 
          grid-cols-1 p-4 gap-y-4
          sm:grid-cols-2 sm:gap-8 sm:py-8
          md:grid-cols-3
          xl:grid-cols-4">
               <img class="w-full aspect-square object-cover transition-transform 
               sm:hover:scale-110"
                    v-for="i in 7"
                    src="https://placehold.co/400x600?text=Foto"
                    alt="">
          </section>
     </div>
</template> 

<style scoped></style> 
