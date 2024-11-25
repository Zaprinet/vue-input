<script setup>
const props = defineProps({
  modelValue: {
    type: String,
  }
})
</script>

<template>
  <input type="image" src=""
    alt=image-input:
    :value="modelValue" @click="(event) => {
    $emit('update:modelValue', event.target.src)}"
    >
</template>

<style>

</style>