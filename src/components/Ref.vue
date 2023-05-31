<script setup>
import { ref } from 'vue';

const state = {
  count: ref(0),
};
</script>

<template>
  <button @click="state.count.value++">count++ = {{ state.count }}</button>
</template>
