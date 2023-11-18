<script setup lang='ts'>
defineProps<{
    title: string
    id: string
    placeholder?: string
}>()
</script> 

<template>
    <fieldset class="flex flex-col">
        <label class="font-bold text-sm"
               :for="id">{{ title }}</label>
        <input class="outline-none p-2 rounded"
               :id="id"
               type="text"
               :placeholder="placeholder">
    </fieldset>
</template> 

<style scoped></style> 
