<template>
  <Navbar/>
  <body>
    <h1>{{sum(2,2)}}</h1>
    <h2>{{greeting('Enrique')}}</h2>
    <Boolean/>
  </body>
  <Footer></Footer>
</template>
<script setup>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
import Boolean from './components/Boolean.vue';

const sum = (num1, num2) => {
    return num1 + num2; 
}

sum(); 

function greeting(name) {
  return `hola ${name}`; 
}

greeting(); 


const getRandom = () => {
    return Math.floor(Math.random() * 255); 
}

const changeBackground = () => {
    backgroundColor = `rgb(${getRandom()}, ${getRandom()}, ${getRandom()})`
}


</script>
<style scoped>