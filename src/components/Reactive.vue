<script setup>
import { reactive } from 'vue';

const state = reactive({ count: 0 });
</script>

<template>
  <button @click="state.count++">count++ = {{ state.count }}</button>
</template>
