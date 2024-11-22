<script setup>
  const props = defineProps({
    modelValue: {
      type: String,
      default: 'Test@101'
    }
  })
</script>

<template>
  <input type="password" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)">
</template>

<style lang="css" scoped></style>