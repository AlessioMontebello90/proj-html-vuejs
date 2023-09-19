<script>
import Logo from "../Logo.vue";
import NavbarMenu from "./NavbarMenu.vue";
import NavbarIcons from "./NavbarIcons.vue";
export default {
  name: "Navbar",
  components: {
    Logo,
    NavbarMenu,
    NavbarIcons,
  },
};
</script>

<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid w-100 justift-content-between">
      <Logo />
      <NavbarMenu />
      <NavbarIcons />
    </div>
  </nav>
</template>

<style scoped lang="scss"></style>
