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
.gaming-arena {
  height: 100vh;
  background-color: #202046;
  background-image: url("../../assets/img/Vector.png");
  display: flex;
  align-items: center;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
