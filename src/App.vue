<template>
  <Count msg="Count" />
  <Grids :rows="10" :cols="9" />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Count from './components/Count.vue'
import Grids from './components/Grids.vue'

export default defineComponent({
  name: 'App',
  components: {
    Count,
    Grids,
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
