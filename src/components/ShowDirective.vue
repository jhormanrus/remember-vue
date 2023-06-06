<script setup>
import { ref } from 'vue';

const hide = ref(false);
</script>

<template>
  <input id="hide" type="checkbox" v-model="hide" />
  <label for="hide">Hide text</label>
  <br />
  <span v-show="!hide"> I'm always here, just display me</span>
</template>
