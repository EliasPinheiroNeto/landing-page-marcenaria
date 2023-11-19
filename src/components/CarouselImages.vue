<script setup lang='ts'>
defineProps<{
    src: string
    alt?: string
}>()
</script> 

<template>
    <div class="flex-shrink-0 w-full px-2 
                sm:w-1/2">
        <img class="w-full"
             :src="src"
             :alt="alt">
    </div>
</template> 

<style scoped></style> 
