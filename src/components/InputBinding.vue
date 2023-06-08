<script setup>
import { ref } from 'vue';

const name = ref('Julian');
const isPerson = ref(true);
const isWorking = ref(false);
const documents = ref(['passport']);
const shortBio = ref('Lorem ipsum\n dolor isamet ...');
</script>

<template>
  <input v-model="name" type="text" />
  <br />
  <span>My name is {{ name }}</span>
  <br />
  <input v-model="isPerson" id="isperson" type="radio" :value="true" />
  <label for="isperson">Is a person</label>
  <input v-model="isPerson" id="isnotperson" type="radio" :value="false" />
  <label for="isnotperson">Isn't a person</label>
  <br />
  <span>I'm a person: {{ isPerson ? 'Yes' : 'No' }}</span>
  <br />
  <select v-model="isWorking" id="status">
    <option :value="true">Working</option>
    <option :value="false">Not working</option>
  </select>
  <br />
  <span>Currently {{ isWorking ? 'working' : 'not working' }}</span>
  <br />
  <input v-model="documents" id="id" type="checkbox" value="id" />
  <label for="id">ID</label>
  <input v-model="documents" id="passport" type="checkbox" value="passport" />
  <label for="passport">Passport</label>
  <br />
  <span>Has documents: {{ documents.join(', ') }}</span>
  <br />
  <textarea v-model="shortBio" rows="2"></textarea>
  <br />
  <span>Short bio: {{ shortBio }}</span>
</template>
