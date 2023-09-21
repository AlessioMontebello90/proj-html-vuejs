<script>
import LinkButton from "./LinkButton.vue";
import PlayButton from "./PlayButton.vue";
export default {
  name: "ButtonComposition",
  components: {
    LinkButton,
    PlayButton,
  },
  props: {
    text: String,
  },
};
</script>

<template>
  <div class="buttons justify-content-center">
    <LinkButton :text="text" />
    <PlayButton />
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.buttons {
  @include center();
}
</style>
