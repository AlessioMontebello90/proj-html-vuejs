<script>
import OurCompany from "./OurCompany/OurCompany.vue";
import GamingArena from "./GamingArena/GamingArena.vue";
import OurStreaming from "./OurStreaming/OurStreaming.vue";
export default {
  name: "AppMain",
  components: {
    OurCompany,
    GamingArena,
    OurStreaming,
  },
};
</script>

<template>
  <OurCompany />
  <GamingArena />
  <OurStreaming />
</template>

<style scoped lang="scss"></style>
