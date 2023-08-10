<script setup lang="ts">
import {ref} from 'vue'
import  HelloWorld  from './HelloWorld.vue'



const helloWorld = ref('Hello World')

</script>

<template>
  <HelloWorld />
  <span>{{ helloWorld }}</span>
</template>
