<script setup>
import { ref } from 'vue';

const count = ref(1);
const message = 'You clicked me';

function handleClick() {
  alert(message);
}

function showTagName(event) {
  alert(event.target.tagName);
}

function showTagName2(showAlert, event) {
  if (!showAlert) return;
  alert(event.target.tagName);
}
</script>

<template>
  <button @click="handleClick()" type="button">Click me</button>
  <button @click="count++" type="button">Count is {{ count }}</button>
  <button @click="showTagName" type="button">I'm a ...</button>
  <button @click="showTagName2(true, $event)" type="button">I'm a ...</button>
</template>
