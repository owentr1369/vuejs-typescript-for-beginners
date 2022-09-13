<template>
  <div class="home">
    <app-header :msg="msg"></app-header>
    <h1>This is home page</h1>
  </div>
</template>

<script lang="ts">
import AppHeader from "@/components/AppHeader.vue";
import { defineComponent, ref } from "vue";

export default defineComponent({
  components: { AppHeader },
  name: "HomeView",
  setup() {
    const msg = ref<string>("Hello this is Vue3 + TypeScript");

    return { msg };
  },
});
</script>
