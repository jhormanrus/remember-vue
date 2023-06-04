<script setup>
import { computed, ref } from 'vue';

const firstName = ref('Jhorman');
const lastName = ref('Tito');

const fullName = computed({
  get() {
    return `${firstName.value} ${lastName.value}`;
  },
  set(newValue) {
    [firstName.value, lastName.value] = newValue.split(' ');
  },
});
</script>

<template>
  <br />
  First name: <input type="text" v-model="firstName" /> <br />
  Last name: <input type="text" v-model="lastName" /> <br />
  Full name: <input type="text" v-model="fullName" />
</template>
