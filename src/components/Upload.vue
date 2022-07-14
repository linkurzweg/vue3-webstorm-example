<template>
  <n-upload
      action="https://www.mocky.io/v2/5e4bafc63100007100d8b70f"
      :headers="{
      'naive-info': 'hello!'
    }"
      :data="{
      'naive-data': 'cool! naive!'
    }"
      :on-error="onError"
  >
    <n-button>Upload File</n-button>
  </n-upload>
</template>

<script setup lang="ts">
import { NUpload } from 'naive-ui'

const onError = () => {
  console.log('Upload failed!')
}
</script>

<style scoped lang="sass"></style>
