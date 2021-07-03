<template>
  <h1>{{ msg }}</h1>

  <p>See <code>README.md</code> for more information.</p>

  <p>
    Built with
    <a href="https://v3.vuejs.org/" target="_blank">Vue</a>
    |
    <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite</a>
  </p>

  <button type="button" @click="count++">Count: {{ count }}</button>
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'
export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      required: true
    }
  },
  setup: () => {
    const count = ref(0)
    return { count }
  }
})
</script>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
