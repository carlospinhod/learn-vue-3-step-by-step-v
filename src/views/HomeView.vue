<script setup>

import TabbableTextarea from '@/components/TabbableTextarea.vue'
import { ref } from 'vue'

let comment = ref('A value!')

</script>

<template>
  <main>
    <TabbableTextarea v-model="comment" style="width: 100%; height: 300px;" />
  </main>
</template>
