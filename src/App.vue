<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";
import Powerslide from "./components/Powerslide.vue";

export default defineComponent({
  name: "App",
  components: {
    Powerslide,
    Header,
  },
});
</script>

<template>
  <div
    class="bg-zinc-800 min-h-screen text-white flex flex-col justify-between p-10"
  >
    <header class="flex">
      <Header />
    </header>
    <main class="flex">
      <Powerslide />
    </main>
    <footer class="flex"></footer>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap");
* {
  font-family: "Roboto", sans-serif;
}
</style>
