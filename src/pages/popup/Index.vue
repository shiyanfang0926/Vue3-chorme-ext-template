<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
    <img alt="Vue logo" src="../../assets/logo.png" @click="handleClick">
    <HelloWorld :msg="msg"/>
  </div>
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue'
import { ref } from 'vue'

const msg = ref('Welcome to Your Vue.js App')
const handleClick = () => {
  if (msg.value === 'Welcome to Your Vue.js App') {
    msg.value = 'You clicked the logo!'
    return
  }
  msg.value = 'Welcome to Your Vue.js App!'
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
