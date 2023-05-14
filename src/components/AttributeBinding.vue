<script setup>
const placeholder = 'binding placeholder';
const nullishPlaceholder = null;
</script>

<template>
  <input type="text" v-bind:placeholder="placeholder" />
  <!-- if bound value is nullish, then it is removed from rendered html -->
  <input type="text" :placeholder="nullishPlaceholder" />
</template>
