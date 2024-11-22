<script setup>
const props = defineProps({
  modelValue: {
    type: Boolean,
    default: true
  },
  inputType: {
    type: String
  }
})

</script>

<template>
  <input :type="inputType" :value="modelValue" @input="(event) => {
      console.log(event.target); // Logs the input value
      $emit('update:modelValue', event.target.checked);
    }" >
</template>

 <style>

</style>