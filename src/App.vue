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
import WritableComputed from './components/WritableComputed.vue';
import ClassBinding from './components/ClassBinding.vue';
import StyleBinding from './components/StyleBinding.vue';
import IfElseDirective from './components/IfElseDirective.vue';
import ShowDirective from './components/ShowDirective.vue';
import ForDirective from './components/ForDirective.vue';
import OnDirective from './components/OnDirective.vue';
import InputBinding from './components/InputBinding.vue';
import TemplateRef from './components/TemplateRef.vue';
import PropsDeclaration from './components/PropsDeclaration.vue';
import PropsDeclaration2 from './components/PropsDeclaration2.vue';
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
    <li>
      <b>Class and style binding:</b>
      <ClassBinding class="border" />
    </li>
    <li>
      <b>Style binding:</b>
      <StyleBinding />
    </li>
    <li>
      <b>If else directive:</b>
      <IfElseDirective />
    </li>
    <li>
      <b>Show directive:</b>
      <ShowDirective />
    </li>
    <li>
      <b>For directive:</b>
      <ForDirective />
    </li>
    <li>
      <b>Event handling:</b>
      <OnDirective />
    </li>
    <li>
      <b>Input binding:</b>
      <InputBinding />
    </li>
    <li>
      <b>Template ref:</b>
      <TemplateRef />
    </li>
    <li>
      <b>Props declaration:</b>
      <PropsDeclaration :index="3" item="Banana" />
      <br />
      <PropsDeclaration2 :item-index="4" :item="{ name: 'Apple' }" is-last />
    </li>
  </ul>
</template>
