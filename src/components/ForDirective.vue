<script setup>
const fruits = [
  {
    id: 1,
    name: 'apple',
    color: 'red',
  },
  {
    id: 2,
    name: 'banana',
    color: 'yellow',
  },
  {
    id: 3,
    name: 'orange',
    color: 'orange',
  },
];
const object = {
  title: 'How to do lists in Vue',
  author: 'Jane Doe',
  publishedAt: '2016-04-10',
};
</script>

<template>
  <ul>
    <li v-for="({ id, name, color }, index) of fruits" :key="id">
      {{ index }} -> {{ name }} is {{ color }}
    </li>
  </ul>
  <hr />
  <ul>
    <li v-for="(value, key) of object">{{ key }}: {{ value }}</li>
  </ul>
  <hr />
  <ul>
    <template v-for="n of 3">
      <li>{{ n }}</li>
    </template>
  </ul>
</template>
