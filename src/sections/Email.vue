<script setup lang='ts'>
import { reactive } from 'vue';

import InputText from '@/components/InputText.vue';
import InputTextarea from '@/components/InputTextarea.vue';

const form = reactive({
    name: "",
    email: "",
    phone: "",
    message: ""
})
</script> 

<template>
    <div class="w-full bg-blue-500"
         id="email">
        <section class="container mx-auto py-8
        flex flex-col-reverse 
        md:grid md:grid-cols-5">
            <form class="bg-gray-200 rounded-md flex flex-col
            mx-4 p-4 gap-y-4
            sm:col-span-3 sm:px-8 sm:gap-y-4 
            lg:ml-8 lg:mr-24">
                <InputText title="NOME: "
                           id="input-name"
                           name="name"
                           placeholder="Digite seu nome"
                           required
                           @update="e => { form.name = e }" />

                <InputText title="E-MAIL: "
                           id="input-email"
                           name="email"
                           placeholder="Digite seu email"
                           required
                           @update="e => { form.email = e }" />

                <InputText title="TELEFONE: "
                           id="input-phone"
                           name="phone"
                           placeholder="Digite seu telefone"
                           @update="e => { form.phone = e }" />

                <InputTextarea title="MENSAGEM: "
                               id="input-message"
                               name="message"
                               placeholder="Digite sua mensagem"
                               @update="e => { form.message = e }" />

                <button class="bg-blue-400 text-white font-bold rounded
                w-full h-12 text-lg
                sm:w-1/4 sm:ml-auto sm:h-8"
                        type="submit">
                    Enviar
                </button>
            </form>
            <div class="sm:my-auto sm:col-span-2">
                <h2 class="text-white text-4xl
                text-center mb-4
                md:text-left md:mb-0">Fale <br class="hidden md:block"><strong class="md:text-5xl">Conosco</strong>
                </h2>
            </div>
        </section>
    </div>
</template> 

<style scoped></style> 

