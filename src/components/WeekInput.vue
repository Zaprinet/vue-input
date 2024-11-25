<script setup>
  

  const props = defineProps({
    modelValue: {
      type: String,
    }
  })
</script>

<template>
  <input type="week" :value="modelValue" @input="(event) => {
    $emit('update:modelValue', event.target.value)
  }">
</template>

<style lang="css" scoped>

</style>