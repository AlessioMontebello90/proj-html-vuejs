<script>
export default {
  name: "PlayButton",
};
</script>

<template>
  <a class="arrow" href="#">
    <img
      class="img-fluid"
      src="../../assets/img/image (9).svg"
      alt="arrow-right"
  /></a>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
a.arrow {
  @include center();
  @include round();
  text-decoration: none;
  color: $darker-blue;
  background-color: $green;
  padding: 20px 22px;
  img {
    height: 20px;
  }
}
</style>
