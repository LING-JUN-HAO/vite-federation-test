<script setup>
import { defineAsyncComponent } from 'vue'

const HelloWorld = defineAsyncComponent(() =>
  import('remote_app/HelloWorld')
)
</script>

<template>
  <div class="container">
    <HelloWorld msg="Vite + Vue A" />
    <HelloWorld msg="Vite + Vue B" />
    <HelloWorld msg="Vite + Vue C" />
    <HelloWorld msg="Vite + Vue D" />
    <HelloWorld msg="Vite + Vue E" />
    <HelloWorld msg="Vite + Vue F" />
  </div>
</template>

<style scoped>
.container{
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
</style>
