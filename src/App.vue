<script setup lang="ts">
import { onBeforeMount, onBeforeUnmount } from 'vue'
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Home from './components/Home.vue'
import MainContent from './components/MainContent.vue'
import UseCase from './components/UseCase.vue'
import MainFeature from './components/MainFeature.vue'
import Compare from './components/Compare.vue'

const scrollFn = () => {

}

onBeforeMount(() => {

})
onBeforeUnmount(() => {

})
</script>

<template>
  <Home />
  <MainContent />
  <UseCase/>
  <MainFeature/>
  <Compare/>
</template>

<style>
body {
  background: #000;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  width: 1200px;
  position: relative;
  left: 50%;
  transform: translate(-50%, 0);
  transition: cubic-bezier(0.075, 0.82, 0.165, 1);
}
body, div, p, span, header, section {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
