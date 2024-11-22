<script setup>
const props = defineProps({
  modelValue: {
    type: String,
    default: 2,
  }
})

</script>

<template>
  <input type="color" placeholder="+234" :value="modelValue" @input="(event) => {
      console.log(event.target); // Logs the input value
      $emit('update:modelValue', event.target.value);
    }" >
</template>

 <style>

</style>