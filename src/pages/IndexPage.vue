<template>
  <q-page class="flex flex-center">
    <div style="width: 30%">
      <q-select label="Input" v-model="model" :options="options"></q-select>
    </div>
    <div style="width: 30%">
      <q-btn label="Menu">
        <q-menu>
          <q-list>
            <q-item
              v-for="n in options"
              :key="n"
              dense
              clickable
            >
              <q-item-section>{{ n }}</q-item-section>
            </q-item>
          </q-list>
        </q-menu>
      </q-btn>
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
