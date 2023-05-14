<script setup>
const text = 'This is <b>bold</b>';
</script>

<template>
  <span v-html="text"></span>
</template>
