<script>
export default {
  name: "OurStreaming",
};
</script>

<template>
  <section class="our-streaming">
    <div class="container">
      <div class="live-stream">
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
.our-streaming {
  height: 80vh;
  background-image: url("../../assets/img/v-bg.png");
  background-size: cover;
  .container {
    height: 100%;
    display: flex;
    align-items: center;
    .live-stream {
      height: 100%;
      display: flex;
      align-items: center;
      flex-basis: 50%;
      figure {
        width: 392px;
        height: 260px;
        position: relative;
      }
      a.arrow {
        display: flex;
        align-items: center;
        justify-content: center;
        text-decoration: none;
        color: $white;
        background-color: $green;
        border-radius: 50%;
        padding: 20px 22px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        img {
          height: 20px;
        }
      }
    }
  }
}
</style>
