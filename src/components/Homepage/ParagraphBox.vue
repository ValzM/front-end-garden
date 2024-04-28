<script setup lang="ts">
import { computed } from 'vue'

const sentence = 'Hello World lorem ipsum'

const sentenceWord = computed(() => sentence.split(' '))
</script>

<template>
  <div class="word-wrapper">
    <div v-for="(word, index) in sentenceWord" :key="index">{{ word }}</div>
  </div>
</template>

<style scoped>
.word-wrapper {
  display: flex;
  gap: 8px;
  color: white;
  font-size: x-large;
}
</style>
