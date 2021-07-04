<template>
  <p class="mt-2 text-sm text-gray-500">{{ fen }} {{ rows }} x {{ cols }} = {{ total }}</p>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "Grids",
  computed: {
    total(): Number {
      return this.rows! * this.cols!;
    }
  },
  props: {
    fen: String,
    rows: Number,
    cols: Number,
  },
  setup: () => {
    return {
    };
  },
});
</script>
