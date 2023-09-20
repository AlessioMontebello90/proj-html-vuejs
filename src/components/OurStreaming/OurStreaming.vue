<script>
export default {
  name: "OurStreaming",
};
</script>

<template>
  <section class="our-streaming">
    <div class="container h-100">
      <div class="live-stream h-100">
        <figure>
          <img
            class="img-fluid"
            src="../../assets/img/v-small1.png"
            alt="Call of deuty"
          />
          <a class="arrow" href="#">
            <img
              class="img-fluid"
              src="../../assets/img/image (9).svg"
              alt="arrow-right"
          /></a>
        </figure>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.our-streaming {
  height: 80vh;
  background-image: url("../../assets/img/v-bg.png");
  background-size: cover;
  .container {
    @include center("cross");
    .live-stream {
      @include center("cross");
      flex-basis: 50%;
      figure {
        width: 392px;
        height: 260px;
        position: relative;
      }
      a.arrow {
        @include center();
        @include round();
        @include absolute-center();
        text-decoration: none;
        color: $white;
        background-color: $green;
        padding: 20px 22px;

        img {
          height: 20px;
        }
      }
    }
  }
}
</style>
