<template>
  <div class="app-header">
    <h1>This is header</h1>
    <p>{{ msg }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from "vue";

export default defineComponent({
  props: {
    msg: {
      required: true,
      type: String as PropType<string>,
    },
  },
});
</script>
