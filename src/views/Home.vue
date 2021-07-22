<template>
  <div class="home">
    <img class="logo" alt="Friendly Inquiry logo" src="../assets/logo.svg" />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Options({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
.home {
  padding: 40px;
}
.logo {
  max-width: 500px;
}
</style>
