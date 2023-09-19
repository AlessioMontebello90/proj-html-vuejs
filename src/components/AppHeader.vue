<script>
import Navbar from "./navbar/Navbar.vue";
export default {
  name: "AppHeader",
  components: {
    Navbar,
  },
};
</script>

<template>
  <header>
    <div class="container">
      <Navbar />
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
