<script setup>
const props = defineProps({
  modelValue: {
    type: String,
    default: 'Prince'
  },

})

</script>

<template>
  <main>
    <input type="text" :value="modelValue"  @input="$emit('update:modelValue', $event.target.value)" >
  </main>
</template>

<style lang="css" scoped>

</style>