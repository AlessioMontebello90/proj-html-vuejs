<script>
import OurCompany from "./OurCompany/OurCompany.vue";
import GamingArena from "./GamingArena/GamingArena.vue";
import OurStreaming from "./OurStreaming/OurStreaming.vue";
import UpcomingMatch from "./UpcomingMatch/UpcomingMatch.vue";
export default {
  name: "AppMain",
  components: {
    OurCompany,
    GamingArena,
    OurStreaming,
    UpcomingMatch,
  },
};
</script>

<template>
  <OurCompany />
  <GamingArena />
  <OurStreaming />
  <UpcomingMatch />
</template>

<style scoped lang="scss"></style>
