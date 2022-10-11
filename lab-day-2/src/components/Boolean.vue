<template>  
    
    <div v-if="activo === true">Estoy activo</div>
    <div v-else="inactivo === false">Estoy inactivo</div>
    <button @click="show()">Click</button>
    
    
    <div v-if="active === true">This element is active</div>
    <div v-show="active === false"></div>
    
    </template>
    <script setup>
    
    import { ref } from 'vue'; 
    
    const activo = ref(true); 
    const inactivo = false; 
    const show = () => {
        activo.value = !activo.value; 
    }
    
    
    const active = true; 
    
    
    </script>
    
    <style scoped>
    </style>