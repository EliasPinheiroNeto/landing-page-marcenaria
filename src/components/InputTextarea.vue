<script setup lang='ts'>
withDefaults(defineProps<{
    title: string
    id: string
    placeholder?: string
    rows?: number
}>(), {
    rows: 5
})
</script> 

<template>
    <fieldset class="flex flex-col">
        <label class="font-bold text-sm"
               :for="id">{{ title }} </label>
        <textarea class="outline-none p-2 rounded resize-none"
                  :id="id"
                  :placeholder="placeholder"
                  :rows="rows"></textarea>
    </fieldset>
</template> 

<style scoped></style> 
