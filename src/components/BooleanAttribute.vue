<script setup>
const truthyValue = 1;
</script>

<template>
  <!-- if attr is boolean, boudn value is treated as truthy value -->
  <input type="checkbox" :checked="truthyValue" />
</template>
