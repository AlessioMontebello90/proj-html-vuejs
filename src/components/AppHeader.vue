<script>
import Navbar from "./navbar/Navbar.vue";
import HeaderJumbo from "./headerjumbo/HeaderJumbo.vue";
import SocialLinks from "./headerjumbo/SocialLinks.vue";
import PlayerIcons from "./headerjumbo/PlayerIcons.vue";

export default {
  name: "AppHeader",
  components: {
    Navbar,
    HeaderJumbo,
    SocialLinks,
    PlayerIcons,
  },
};
</script>

<template>
  <header>
    <div class="container">
      <Navbar />
      <SocialLinks />
      <HeaderJumbo />
      <PlayerIcons />
    </div>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 95vh;
  background-image: url("../assets/img/banner1.png");
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
</style>
