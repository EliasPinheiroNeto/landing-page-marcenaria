<script setup lang='ts'>
const phone = "5511999068489"
const message = "Bom dia"

const url = `https://wa.me//${phone}?text=${message.replace(/ /g, '%20')}`
</script> 

<template>
    <a class="fixed bottom-4 right-4 w-12 h-12 hover:scale-105 transition-transform"
       aria-label="Chat on Watsapp"
       :href="url"
       target="_blank">
        <img src="../assets/zap_icon.png"
             alt="Whatsapp icon">
    </a>
</template> 

<style scoped></style> 
