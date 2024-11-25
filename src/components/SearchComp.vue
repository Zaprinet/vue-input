<script setup>
import { ref } from 'vue';
import CheckboxComp from './CheckboxComp.vue';
import InputComp from './InputComp.vue';
import SelectComp from './SelectComp.vue';
import Telnput from './Telnput.vue';
import ColorInputComp from './ColorInputComp.vue';
import DateInput from './DateInput.vue';
import FileInput from './FileInput.vue';
import RadioInput from './RadioInput.vue';
import PasswordComp from './PasswordComp.vue';
import RangeComp from './RangeComp.vue';
import ImageInput from './ImageInput.vue';
import SubmitInput from './SubmitInput.vue';
import TimeInput from './TimeInput.vue';
import WeekInput from './WeekInput.vue';
import UrlInput from './UrlInput.vue';


const newModel = ref('Prince')
const isChecked = ref(false)
const newCar = ref('opel')
const newPhoneNo = ref(null)
const newColor = ref(null)
const newDate = ref('2020-02-20')
const newFile = ref(null )
const newValue = ref(false)
const newPassword = ref('Test@101')
const newRange = ref('')
const newImage = ref('')
const newSubmit = ref('Submit')
const newWeek = ref('Week 44, 2024')
const input = ref('radio')
const newTime = ref('00:01')
const newUrl = ref('www.abaaly.com')

</script>

<template>
  <InputComp v-model="newModel"/>
  <p>{{ newModel }}</p>

  <CheckboxComp v-model="isChecked" />
  <p>{{ isChecked }}</p>

  <SelectComp v-model="newCar"/>
  <p>{{ newCar }}</p>

  <Telnput v-model="newPhoneNo"/>
  <p>{{ newPhoneNo }}</p>

  <ColorInputComp v-model="newColor" />
  <p>{{ newColor }}</p>

  <DateInput v-model="newDate" />
  <p>{{ newDate }}</p>

  <FileInput v-model="newFile" />
  <p>{{ newFile }}</p>

  <RadioInput v-model="newValue" :type="input"/>
  <p>{{ newValue }}</p>

  <PasswordComp v-model="newPassword" />
  <br>
  {{ newPassword }}
  <hr>

  <RangeComp v-model="newRange" />
  {{ newRange }}
  <br>

  <ImageInput v-model="newImage"/>
  {{ newImage }}
  <br>

  <SubmitInput v-model="newSubmit" />
  {{ newSubmit }}
  <br>

  <TimeInput v-model="newTime"/>
  {{ newTime }}
  <br>

  <WeekInput v-model="newWeek"/>
  {{ newWeek }}
  <br>

  <UrlInput v-model="newUrl" />
  {{ newUrl }}
</template>

<style lang="css" scoped>

</style>