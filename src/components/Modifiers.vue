<script setup>
function onSubmit(e) {
  alert(e.type);
}
</script>

<template>
  <form @submit.prevent="onSubmit">
    <button type="submit">Submit</button>
  </form>
</template>
