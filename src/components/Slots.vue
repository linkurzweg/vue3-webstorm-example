<template>
  <n-card title="Card Slots Demo">
    <template #header-extra> #header-extra </template>
    Card Content
    <template #footer> #footer </template>
    <template #action> #action </template>
  </n-card>
</template>

<script setup lang="ts">
import { NCard } from 'naive-ui'
</script>