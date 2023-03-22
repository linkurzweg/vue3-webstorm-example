<script setup lang="ts">
import { NH1 } from 'naive-ui'
import { useStore } from '../store/store'

const store = useStore()

import { useAxios } from '@vueuse/integrations/useAxios'
import Fact from './Fact.vue'

const { data, isFinished } = useAxios<{ fact: string, length: number}>('https://catfact.ninja/fact')
</script>

<template>
  <n-h1>{{ store.headline }}</n-h1>
  <Fact :data="data" v-if="isFinished" />
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
