<template>
  <div>
    {{name}}
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

defineProps({
  msg: String
})
</script>

<style scoped>

</style>
