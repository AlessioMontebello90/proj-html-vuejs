<script>
import OurCompany from "./OurCompany/OurCompany.vue";
import GamingArena from "./GamingArena/GamingArena.vue";
import OurStreaming from "./OurStreaming/OurStreaming.vue";
import UpcomingMatch from "./UpcomingMatch/UpcomingMatch.vue";
import TrendingGames from "./TrendingGames/TrendingGames.vue";
import Matches from "./Matches/Matches.vue";
import OurExperts from "./OurExpert/OurExperts.vue";
import Testimonials from "./Testimonials/Testimonials.vue";
export default {
  name: "AppMain",
  components: {
    OurCompany,
    GamingArena,
    OurStreaming,
    UpcomingMatch,
    TrendingGames,
    Matches,
    OurExperts,
    Testimonials,
  },
};
</script>
<template>
  <OurCompany />
  <GamingArena />
  <OurStreaming />
  <UpcomingMatch />
  <TrendingGames />
  <Matches />
  <OurExperts />
  <Testimonials />
</template>

<style scoped lang="scss"></style>
