<script setup lang='ts'>
import { ref } from 'vue';

defineProps<{
    title: string
    id: string
    placeholder?: string
    name?: string
    required?: boolean
}>()

defineEmits<{
    (event: 'update', data: string): void
}>()

const data = ref("")
</script> 

<template>
    <fieldset class="flex flex-col">
        <label class="font-bold text-sm"
               :for="id">{{ title }}</label>
        <input class="outline-none p-2 rounded"
               :id="id"
               :name="name"
               :required="required"
               type="text"
               :placeholder="placeholder"
               v-model="data"
               @input="$emit('update', data)">
    </fieldset>
</template> 

<style scoped></style> 
