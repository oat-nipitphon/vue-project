<template>
  <div class="about grid-rows-2">
    <h1>This is an about page</h1>
    <div class="grid grid-cols-3">
      <h1>{{ form.email }}</h1>
      <h1>{{ labelTitle }}</h1>
      <h1>{{ form.username }}</h1>
    </div>
  </div>
  <div class="flex justify-center m-auto h-50%">
    <div class="grid grid-cols-2">
      <base-input class="text-red-500" type="text" placeholder="input .... " v-model="labelTitle" />
      <base-input class="text-red-500" type="text" placeholder="input .... " v-model="form.email" />
      <base-input class="text-red-500" type="text" placeholder="input .... " v-model="form.username" />
    </div>
  </div>
</template>
<script setup>
import { ref, reactive } from 'vue';
import BaseInput from '@/components/BaseInput.vue';

const labelTitle = ref("");
const form = reactive({
  username: "web_developer",
  email: "develoment@dev.web",
});

</script>
<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
