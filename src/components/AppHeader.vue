<script>
import Navbar from "./navbar/Navbar.vue";
import HeaderJumbo from "./headerjumbo/HeaderJumbo.vue";
export default {
  name: "AppHeader",
  components: {
    Navbar,
    HeaderJumbo,
  },
};
</script>

<template>
  <header>
    <div class="container">
      <Navbar />
      <HeaderJumbo />
    </div>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 90vh;
  background-image: url("../assets/img/banner1.png");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
