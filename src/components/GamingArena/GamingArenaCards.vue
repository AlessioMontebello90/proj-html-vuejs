<script>
import ArenaCard from "./ArenaCard.vue";
export default {
  name: "GamingArenaCards",
  components: {
    ArenaCard,
  },
};
</script>

<template>
  <div class="arena-cards-list">
    <ArenaCard />
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
.arena-cards-list {
  @include center("cross");
  height: 70%;
  flex-basis: 45%;
  flex-wrap: wrap;
}
</style>
