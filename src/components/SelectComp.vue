<script setup>
const props = defineProps({
  modelValue: {
    type: String,
    default: 'opel'
  }
})


</script>

 <template>
  <select name="cars" id="cars" form="carform" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="opel">Opel</option>
    <option value="audi">Audi</option>
  </select>
{{ modelValue }}
 </template>

 <style lang="css" scoped>

</style>

