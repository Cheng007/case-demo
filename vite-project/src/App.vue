<script setup lang="ts">
import { ref } from 'vue'
import Reactive from './components/Reactive.vue'
import LifeUpdate from './components/LifeUpdate.vue'
import Composition from './components/Composition.vue'

let count = ref(1)
const onClick = () => {
  count.value += 1
}
</script>

<template>
  响应式demo
  <button @click="onClick">Count 加 1</button>
  <Reactive :count="count" />
  <LifeUpdate />
  <Composition />
</template>

<style scoped>
</style>
