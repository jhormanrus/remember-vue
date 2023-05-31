<script setup>
import { computed, ref } from 'vue';

const x = ref(3);
const y = ref(5);

const result = computed(() => x.value + y.value);
</script>

<template>
  <input v-model="x" type="number" />
  +
  <input v-model="y" type="number" />
  =
  {{ result }}
</template>
