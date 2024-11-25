<script setup>
const props= defineProps({
  modelValue: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <input type="submit" name="name"
  :value="modelValue" @click="(event) => {
    console.log(event.target);
    $emit('update:modelValue', event.target.value)}"/>
</template>

<style lang="css" scoped>

</style>