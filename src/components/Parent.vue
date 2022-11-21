<script setup>
  import { ref } from 'vue'
  import ChildComponent from './Child.vue'
  const count = ref(0)
</script>

<template>
  <ChildComponent @add="(i) => count += i" /> 
  <p>Count: {{ count }}</p>
</template>
