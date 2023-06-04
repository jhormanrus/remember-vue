<script setup>
import { reactive, ref } from 'vue';

const background = ref('blue');

const styles1 = {
  color: 'black',
  backgroundColor: 'yellow',
};

const styles2 = reactive({
  border: '1px solid #000',
});
</script>

<template>
  <div :style="[styles1, styles2]">Yellow box</div>
  <div :style="{ backgroundColor: background }">Blue box</div>

  <input id="blue" type="radio" v-model="background" value="blue" />
  <label for="blue"> Set blue </label>
  <input id="black" type="radio" v-model="background" value="black" />
  <label for="black"> Set black </label>
</template>

<style scoped>
div {
  width: 50px;
  height: 50px;
  color: white;
}
</style>
