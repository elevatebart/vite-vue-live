<script setup lang="ts">
import { VueLive } from 'vue-live'
// if you are using vue-cli, you have to import the css separately
import "vue-live/lib/vue-live.esm.css";
import "prismjs/themes/prism-tomorrow.css";

const code = `
let cool = 12

<center>
  <button style="width:100px" @click="cool++">{{ cool }}</button>
</center>
`
</script>

<template>
  <div style="width:70vw;margin:50px auto; border:1px solid #ccc; padding:20px; border-radius: 20px;">
    <VueLive :code="code" />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap");

.prism-editor-wrapper {
  font-family: "Roboto Mono", monospace;
  background-color: #222;
  color: #eee;
  padding: 8px 12px;
  box-sizing: border-box;
}
</style>
