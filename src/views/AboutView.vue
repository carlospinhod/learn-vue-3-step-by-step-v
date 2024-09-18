<script setup>
import { useFlash } from '@/composables/useFlash';

let { flash } = useFlash();

</script>

<template>
  <div class="about">
    <p>
      <button @click="flash('about', 'It Works About Page!', 'info')">Click me</button>
    </p>
  </div>
</template>