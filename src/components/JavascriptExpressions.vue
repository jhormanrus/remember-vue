<script setup>
let percent = 10;

function percentValue() {
  return `${percent}%`;
}
</script>

<template>
  <!-- functions will be called every time component updates -->
  <button :title="percentValue()">Percentage: {{ percentValue() }}</button>
</template>
