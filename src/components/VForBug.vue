<script setup lang="ts">
import {ref} from 'vue'
const testArr = ref([1, 2, 3, 4, 5, 6, 7, 8, 9])
</script>

<template>
  <div v-for="entry in testArr.filter(entry => entry < 10)">{{ entry }}</div>
</template>
