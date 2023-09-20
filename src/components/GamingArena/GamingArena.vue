<script>
import GamingArenaInfo from "./GamingArenaInfo.vue";
import GamingArenaCards from "./GamingArenaCards.vue";
export default {
  name: "GamingArena",
  components: {
    GamingArenaInfo,
    GamingArenaCards,
  },
};
</script>

<template>
  <section class="gaming-arena">
    <div class="container">
      <GamingArenaInfo />
      <GamingArenaCards />
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.gaming-arena {
  @include center("cross");
  height: 100vh;
  background-color: $darker-blue;
  background-image: url("../../assets/img/Vector.png");

  .container {
    @include center("c-between");
    height: 100%;
  }
}
</style>
