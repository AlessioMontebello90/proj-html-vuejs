<script>
export default {
  name: "Jumbo Social",
};
</script>

<template>
  <div class="social-links">
    <figure>
      <img
        class="img-fluid"
        src="../../assets/img/image (4).svg"
        alt="facebook"
      />
    </figure>
    <figure>
      <img
        class="img-fluid"
        src="../../assets/img/image (5).svg"
        alt="twitter"
      />
    </figure>
    <figure>
      <img
        class="img-fluid"
        src="../../assets/img/image (6).svg"
        alt="linkedin"
      />
    </figure>
    <figure>
      <img
        class="img-fluid"
        src="../../assets/img/image (7).svg"
        alt="instagram"
      />
    </figure>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.social-links {
  position: absolute;
  top: 42%;
  left: 50px;
  figure {
    @include center();
    @include round();
    width: 50px;
    height: 50px;
    background-color: $darker-blue;
    &:hover {
      background-color: $green;
    }
    img {
      height: 20px;
      filter: invert(100%) sepia(10%) saturate(2%) hue-rotate(312deg)
        brightness(112%) contrast(100%);
    }
  }
}
</style>
