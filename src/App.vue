<script setup>
import TextInterpolation from './components/TextInterpolation.vue';
import RawHtml from './components/RawHtml.vue';
import AttributeBinding from './components/AttributeBinding.vue';
import BooleanAttribute from './components/BooleanAttribute.vue';
import MultipleAttributes from './components/MultipleAttributes.vue';
</script>

<template>
  <ul class="list">
    <li>
      <b>Text interpolation:</b>
      <TextInterpolation />
    </li>
    <li>
      <b>Raw HTML:</b>
      <RawHtml />
    </li>
    <li>
      <b>Attribute binding:</b>
      <AttributeBinding />
    </li>
    <li>
      <b>Boolean attribute:</b>
      <BooleanAttribute />
    </li>
    <li>
      <b>Multiple attributes:</b>
      <MultipleAttributes />
    </li>
  </ul>
</template>
