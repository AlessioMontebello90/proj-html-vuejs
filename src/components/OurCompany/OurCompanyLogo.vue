<script>
export default {
  name: "OurCompanyLogo",
};
</script>

<template>
  <div class="logo">
    <figure>
      <img
        id="top-img"
        class="img-fluid"
        src="../../assets/img/exprince.jpg"
        alt="exprince"
      />
      <img
        id="top-shape"
        class="img-fluid"
        src="../../assets/img/exprience-shape.png"
        alt="exprience-shape"
      />
      <img
        id="bottom-square"
        class="img-fluid"
        src="../../assets/img/shape2.png"
        alt="shape2"
      />
      <img
        id="bottom-rettangular"
        class="img-fluid"
        src="../../assets/img/shape1.png"
        alt="shape1"
      />
    </figure>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
.logo {
  flex-basis: 50%;
  position: relative;
  figure {
    height: 100%;
    #top-img {
      height: 450px;
      z-index: 1;
      @include absolute-center();
    }
    #top-shape {
      position: absolute;
      z-index: 1;
      top: 10%;
      left: -5%;
    }
    #bottom-square {
      position: absolute;
      bottom: 8%;
      right: 10%;
    }
    #bottom-rettangular {
      height: 350px;
      position: absolute;
      top: 7%;
      left: 7%;
    }
  }
}
</style>
