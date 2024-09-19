<script setup>
import { useStorage } from '@/composables/useStorage.js'

let food = useStorage('food', 'steak')
let age = useStorage('age')

let obj = useStorage('obj', { one: 'one' })

setTimeout(() => {
  obj.value.one = 'changed'
}, 3000)
</script>

<template>
  <main>
    <p>
      What is your favorite food? <input type="text" v-model="food">
    </p>
    <p>
      How old are you? <input type="text" v-model="age">
    </p>

  </main>
</template>