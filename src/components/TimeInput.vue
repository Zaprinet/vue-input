<script setup>
const props = defineProps({
  modelValue: {
    type: String,
  }
})
</script>

<template>
  <input type="time" :value="modelValue" @input="(event) => {
    console.log(event.target);
    $emit('update:modelValue', event.target.value)
  }">
</template>

<style lang="css" scoped>

</style>