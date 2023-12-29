<script setup lang="ts">
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <v-card
      class="mx-auto"
      width="400"

  >
    <v-btn type="button" @click="count++">count is {{ count }}</v-btn>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </v-card>
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
