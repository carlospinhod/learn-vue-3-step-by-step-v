<script setup>
import TheWelcome from '@/components/TheWelcome.vue'
import { ref } from 'vue'

let message = ref('Hello World!')

let doSomething = () => {
  alert('doing it now')
}
setTimeout(() => {
  message.value = 'I have been changed'
}, 2000)

</script>

<template>
  <main>
    <TheWelcome />
    <p> {{ message }} </p>
    <p>
      <input type="text" v-model="message">
    </p>
    <p>
      <button @click="doSomething">Click me!</button>
    </p>
  </main>
</template>
