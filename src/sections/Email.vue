<script setup lang='ts'>
import InputText from '@/components/InputText.vue';
import InputTextarea from '@/components/InputTextarea.vue';
</script> 

<template>
    <div class="w-full bg-blue-400">
        <section class="container mx-auto grid grid-cols-5 py-8">
            <form class="col-span-3 bg-gray-200 rounded-md mx-8 p-8 flex flex-col gap-y-4">
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
            <div class="my-auto">
                <h2 class="sm:text-4xl text-white">Fale <br><strong class="sm:text-5xl">Conosco</strong></h2>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 

