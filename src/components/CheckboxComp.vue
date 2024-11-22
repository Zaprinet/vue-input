<script setup>
const props = defineProps({
  modelValue: {
    type: Boolean,
    default: false
  },
})


</script>

<template>
<input type="checkbox" :value="modelValue" 
@input="$emit('update:modelValue', $event.target.checked)" >
{{ modelValue }} 
</template>

<style lang="css" scoped>

</style>