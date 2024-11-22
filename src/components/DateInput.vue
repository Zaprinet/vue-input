<script setup>
const props = defineProps({
  modelValue: {
    type: String,
  }
})

</script>

<template>
  <input type="date" :value="modelValue" @input="(event) => {
      console.log(event.target); // Logs the input value
      $emit('update:modelValue', event.target.value);
    }" >
</template>

 <style>

</style>