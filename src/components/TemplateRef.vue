<script setup>
import { onMounted, ref } from 'vue';

const input = ref(null);
const list = ref([]);

onMounted(() => {
  console.log(list.value);
});

function focusInput() {
  input.value.focus();
}

function inputValue(el) {
  console.log(el.value);
}
</script>

<template>
  <input ref="input" type="text" />
  <button @click="focusInput">Focus input</button>
  <br />
  <ul>
    <li v-for="fruit in ['Apple', 'Banana']" ref="list">{{ fruit }}</li>
  </ul>
  <input :ref="inputValue" type="text" value="Hello" />
</template>
