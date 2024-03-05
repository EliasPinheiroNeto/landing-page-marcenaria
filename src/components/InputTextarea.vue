<script setup lang='ts'>
import { ref } from 'vue';

withDefaults(defineProps<{
    title: string
    id: string
    placeholder?: string
    name?: string
    rows?: number
    required?: boolean
}>(), {
    rows: 5
})

defineEmits<{
    (event: 'update', data: string): void
}>()

const data = ref("")
</script> 

<template>
    <fieldset class="flex flex-col">
        <label class="font-bold text-sm"
               :for="id">{{ title }} </label>
        <textarea class="outline-none p-2 rounded resize-none"
                  :id="id"
                  :name="name"
                  :placeholder="placeholder"
                  :rows="rows"
                  :required="required"
                  v-model="data"
                  @input="$emit('update', data)"></textarea>
    </fieldset>
</template> 

<style scoped></style> 
