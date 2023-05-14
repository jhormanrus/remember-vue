<script setup>
const attributes = {
  value: 'Button',
  disabled: true,
};
</script>

<template>
  <input type="button" v-bind="attributes" />
</template>
