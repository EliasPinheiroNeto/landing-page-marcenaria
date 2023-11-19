<script setup lang="ts">
const aboutText = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias optio vitae voluptates earuvoluptate commodi ipsum eius! Voluptate eum magni aspernatur laborum architecto possimus minima, asperiores, exercitationem inventore, suscipit repellendus.Lorem ipsum dolor sit amet consectetur adipisicing elit.Amet, est asperiores nesciunt reiciendis eius eligendi nulla quam sit voluptas nisi eaque rem esse, doloremque quis magni.Neque similique sunt porro.Lorem ipsum dolor sit ametconsectetur adipisicing elit.Lorem ipsum dolor sit, amet consectetur adipisicing elit.Assumendarecusandae ducimus illo itaque incidunt quo quidem ut.Molestias, inventore rem ipsam officiis fugit eligendi, ad, blanditiis numquam voluptatum earum repellendus."
</script> 

<template>
    <div class="w-full">
        <section class="container grid mx-auto p-8 grid-cols-2">
            <div class="my-auto">
                <h2 class="text-4xl">Quem Somos?</h2>
                <p class="mt-8
                hidden
                sm:inline-block">{{ aboutText }}</p>
            </div>

            <div class="relative flex justify-center">
                <div class="absolute aspect-square border-blue-500
                -translate-x-2 translate-y-2 border-2 w-full 
                sm:border-4 sm:-translate-x-4 sm:translate-y-4 sm:w-2/3"></div>

                <img class="h-fit aspect-square object-cover
                w-full
                sm:w-2/3"
                     src="https://placehold.co/400x600?text=Imagem"
                     alt="">
            </div>

            <div class="col-span-2 mt-6 text-center
            block
            sm:hidden">
                <p>{{ aboutText }}</p>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 
