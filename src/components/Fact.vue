<template>
  <div>{{ data.fact }}</div>
</template>

<script setup lang="ts">
const props = defineProps<{ data?: { fact: string, length: number}}>()
</script>

<style scoped lang="sass"></style>
