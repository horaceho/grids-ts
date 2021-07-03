<template>
  <h1 class="text-2xl text-gray-750">{{ msg }}</h1>

  <p class="mt-2 text-sm text-gray-500">See <code>README.md</code> for more information.</p>

  <p class="mt-2 text-sm text-gray-500">
    Built with
    <a href="https://v3.vuejs.org/" target="_blank">Vue</a>
    |
    <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite</a>
  </p>

  
  <div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-md flex items-center space-x-4">
    <div class="flex-shrink-0" @click="count++">
      <img class="h-12 w-12" src="../assets/logo.png" width="32" height="32" alt="horaceho.com">
    </div>
    <div>
      <p class="text-gray-500">Like the icon? Click it to add {{ count }} ...</p>
    </div>
  </div>
</template>

<script lang="ts">
import { ref, defineComponent } from "vue";
export default defineComponent({
  name: "HelloWorld",
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
  setup: () => {
    const count = ref(0);
    return { count };
  },
});
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
