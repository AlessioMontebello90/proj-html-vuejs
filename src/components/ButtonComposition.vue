<script>
export default {
  name: "ButtonComposition",
  props: {
    text: String,
  },
};
</script>

<template>
  <div class="buttons justify-content-center">
    <a class="read" href="#"
      ><b>{{ text }} More </b>
      <img
        class="img-fluid"
        src="../assets/img/image (8).svg"
        alt="arrow-right"
    /></a>
    <a class="arrow" href="#">
      <img
        class="img-fluid"
        src="../assets/img/image (9).svg"
        alt="arrow-right"
    /></a>
  </div>
</template>

<style scoped lang="scss">
@use "../assets/scss/variables" as *;
@use "../assets/scss/mixins" as *;
.buttons {
  @include center();
  a.read {
    text-decoration: none;
    color: $darker-blue;
    background-color: $green;
    border-radius: 10px;
    padding: 15px 30px;
    margin: 0 20px;
    img {
      height: 18px;
    }
  }
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
}
</style>
