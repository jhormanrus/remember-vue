<script setup>
const googleLink = 'https://google.com';

function showAlert() {
  alert(googleLink);
}
</script>

<template>
  <a :href="googleLink">Google</a>
  <button @click="showAlert">Show link</button>
</template>
