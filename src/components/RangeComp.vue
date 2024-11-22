<script setup>
const props = defineProps({
  modelValue: {
    type: Number,
  }
})
</script>

<template>
  <input type="range" :value="modelValue" @input="(event) => {
    console.log(event.target)
    $emit('update:modelValue', event.target.value)}"
  >
</template>

<style>

</style>