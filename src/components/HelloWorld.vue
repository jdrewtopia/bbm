<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);

const serverHello = ref({});

fetch(`/api/v1/hello`)
    .then((r) => r.json())
    .then(({ message }) => {
      serverHello.value = message;
    });
</script>

<template>
  <h1>{{ msg }}</h1>
  <h2>{{ serverHello }}</h2>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    For Benson, Breana, Christiana, John
  </p>
  <p>
    Install
    <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>