<script setup lang="ts">
import HelloWorld from './components/HelloWorld.tsx'
import A from './components/a.vue'
import { stylePxToVw } from '../../../src/index'

console.log("stylePxToVw('300px')",stylePxToVw('300px'))
</script>

<template>
  <div>
    <h3 style="font-size: 28px;margin-top: 10px;width:500px" class="mt-[20px]" :style="{
      width:'1000px'
      }">Test</h3>

<h3 style="
    font-size: 28px;
    margin-top: 10px;
    width:500px;">
    Test</h3>

<h3 
  :style="{fontSize:'28px',marginTop: '10px'}">
Test</h3>
  </div>
  <HelloWorld msg="tsx" />
  <A/>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
