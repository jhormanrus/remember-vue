<script setup>
const props = defineProps({
  itemIndex: [Number, String],
  item: {
    type: Object,
    default(rawProps) {
      console.log(rawProps);
      return { name: 'Apple' };
    },
    validator(value) {
      return ['Apple', 'Banana'].includes(value.name);
    },
  },
  isLast: {
    type: Boolean,
    required: true,
  },
  callback: {
    type: Function,
  },
});
</script>

<template>
  {{ props.itemIndex }} -> {{ props.item.name }} {{ isLast ? 'last' : '' }}
  {{ props.callback() }}
</template>
