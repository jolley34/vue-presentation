<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Header",
});
</script>

<template>
  <div class="flex gap-2 items-center">
    <div class="flex items-center gap-2">
      <h1 class="text-2xl">Vue.js</h1>
      <img
        src="https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png"
        alt=""
        srcset=""
        class="size-5"
      />
    </div>
    <div class="flex">Built with Vue.js OFC</div>
  </div>
</template>

<style scoped></style>
