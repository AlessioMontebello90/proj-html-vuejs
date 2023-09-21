<script>
import OurCompany from "./OurCompany/OurCompany.vue";
import GamingArena from "./GamingArena/GamingArena.vue";
import OurStreaming from "./OurStreaming/OurStreaming.vue";
import UpcomingMatch from "./UpcomingMatch/UpcomingMatch.vue";
import TrendingGames from "./TrendingGames/TrendingGames.vue";
export default {
  name: "AppMain",
  components: {
    OurCompany,
    GamingArena,
    OurStreaming,
    UpcomingMatch,
    TrendingGames,
  },
};
</script>

<template>
  <OurCompany />
  <GamingArena />
  <OurStreaming />
  <UpcomingMatch />
  <TrendingGames />
</template>

<style scoped lang="scss"></style>
