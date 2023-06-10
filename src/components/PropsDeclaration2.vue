<script setup>
const props = defineProps({
  itemIndex: Number,
  item: Object,
  isLast: Boolean,
});
</script>

<template>
  {{ props.itemIndex }} -> {{ props.item.name }} {{ isLast ? 'last' : '' }}
</template>
