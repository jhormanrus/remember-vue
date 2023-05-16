<script setup>
const bindDirective = 'href';
const onDirective = 'click';

const googleLink = 'https://google.com';

function showAlert() {
  alert(googleLink);
}
</script>

<template>
  <a :[bindDirective]="googleLink">Google</a>
  <button @[onDirective]="showAlert">Show link</button>
  <!-- null (and any other non string) will remove the binding -->
  <a :[null]="googleLink">Link</a>
</template>
