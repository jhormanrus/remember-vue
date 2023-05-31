<script setup>
import TextInterpolation from './components/TextInterpolation.vue';
import RawHtml from './components/RawHtml.vue';
import AttributeBinding from './components/AttributeBinding.vue';
import BooleanAttribute from './components/BooleanAttribute.vue';
import MultipleAttributes from './components/MultipleAttributes.vue';
import JavascriptExpressions from './components/JavascriptExpressions.vue';
import DirectiveArguments from './components/DirectiveArguments.vue';
import DinamicArguments from './components/DinamicArguments.vue';
import Modifiers from './components/Modifiers.vue';
import Reactive from './components/Reactive.vue';
import Ref from './components/Ref.vue';
import Computed from './components/Computed.vue';
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
    <li>
      <b>Javascript expressions:</b>
      <JavascriptExpressions />
    </li>
    <li>
      <b>Directive arguments:</b>
      <DirectiveArguments />
    </li>
    <li>
      <b>Dinamic directive arguments:</b>
      <DinamicArguments />
    </li>
    <li>
      <b>Directive modifiers:</b>
      <Modifiers />
    </li>
    <li>
      <b>Reactive:</b>
      <Reactive />
    </li>
    <li>
      <b>Ref:</b>
      <Ref />
    </li>
    <li>
      <b>Computed:</b>
      <Computed />
    </li>
  </ul>
</template>
