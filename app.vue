<script setup lang="ts">
import { useCounterStore } from './stores/counterStore';

const counterStore = useCounterStore();

</script>

<template>
  <div>
    {{ counterStore.counter }}
    <button @click="counterStore.increment">+</button>
    <button @click="counterStore.decrement">-</button>
  </div>
</template>
