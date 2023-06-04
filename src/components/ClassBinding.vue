<template>
  <div class="text-white" :class="{ 'red-box': true, border: true }">
    Red box
  </div>
  <!-- use "$attrs.class" when component has multiple root elements -->
  <div :class="[$attrs.class, 'green-box', { 'text-white': true }]">
    Green box
  </div>
</template>

<style scoped>
div {
  width: 50px;
  height: 50px;
}
.red-box {
  background-color: red;
}
.green-box {
  background-color: green;
}
.border {
  border: 1px solid #000;
}
.text-white {
  color: #fff;
}
</style>
