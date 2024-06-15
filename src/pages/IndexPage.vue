<template>
  <q-page class="flex flex-center">
    <div style="width: 50%">
      <q-select label="Input" v-model="model" :options="options"></q-select>
    </div>

  </q-page>
</template>

<script setup>
import {ref} from "vue";

defineOptions({
  name: 'IndexPage'
});
const model = ref(null);
const options = [
  'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle',
  'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle',
  'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle',
  'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle'
];
</script>
