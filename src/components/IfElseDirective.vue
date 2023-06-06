<script setup>
import { ref } from 'vue';

const name = ref(null);
</script>

<template>
  <br />
  <input id="pedro" type="radio" v-model="name" value="Pedro" />
  <label for="pedro">Pedro</label>
  <br />
  <input id="juan" type="radio" v-model="name" value="Juan" />
  <label for="juan">Juan</label>
  <br />
  <span v-if="name === 'Pedro'">Hello Pedro!</span>
  <span v-else-if="name === 'Juan'">Hello Juan!</span>
  <span v-else>Select an user</span>
  <template v-if="name">Welcome</template>
</template>
