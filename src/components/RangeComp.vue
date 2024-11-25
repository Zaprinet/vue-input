<script setup>
const props = defineProps({
  modelValue: {
    type: String,
  }
})
</script>

<template>
  <input type="range" :value="modelValue" @input="(event) => {
    $emit('update:modelValue', event.target.value)}"
  >
</template>

<style>

</style>