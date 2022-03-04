<template>
  <div>
    Count: {{ count }}
    <div>
      <button @click="decrement" id="decrement">Decrement</button>
      <button @click="increment" id="increment">Increment</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);

function decrement() {
  count.value--
}

function increment() {
  count.value++
}
</script>
