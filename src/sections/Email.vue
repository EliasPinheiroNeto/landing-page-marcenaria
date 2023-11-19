<script setup lang='ts'>
import InputText from '@/components/InputText.vue';
import InputTextarea from '@/components/InputTextarea.vue';
</script> 

<template>
    <div class="w-full bg-blue-500">
        <section class="container mx-auto py-8
        flex flex-col-reverse 
        sm:grid sm:grid-cols-5">
            <form class="bg-gray-200 rounded-md flex flex-col
            mx-4 p-4 gap-y-4
            sm:col-span-3 sm:p-8 sm:gap-y-4 
            lg:ml-8 lg:mr-24">
                <InputText title="NOME: "
                           id="input-name"
                           placeholder="Digite seu nome" />

                <InputText title="EMAIL: "
                           id="input-email"
                           placeholder="Digite seu email" />

                <InputText title="SAPATO: "
                           id="input-"
                           placeholder="Digite seu" />

                <InputTextarea title="MENSAGEM: "
                               id="input-message"
                               placeholder="Digite sua mensagem" />
            </form>
            <div class="sm:my-auto sm:col-span-2">
                <h2 class="text-white text-4xl
                text-center mb-4
                sm:text-left sm:mb-0">Fale <br class="hidden sm:block"><strong class="sm:text-5xl">Conosco</strong>
                </h2>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 

