<template>
  <h1 class="text-6xl font-thin text-green-700 text-center">{{ msg }}</h1>
</template>

<script setup>
import { defineProps } from 'vue'
defineProps({
  msg: {
    type: String,
    default: 'Custom Title',
  },
})
</script>
