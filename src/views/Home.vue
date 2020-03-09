<template>
<v-container>
  <div class="home">
    <img alt="" src="../assets/logo-oasis.png" />
    <HelloWorld msg="Bienvenidos al Hotel Oasis" />
  </div>
</v-container>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>

<style scoped>
img {
  height: 130px;
  width: 160px;
}
</style>
