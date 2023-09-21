<script>
export default {
  name: "TestimonialsList",
};
</script>

<template>
  <div class="testimonials-list d-flex justify-content-center">
    <figure>
      <img src="../../assets/img/test1.png" alt="test" />
    </figure>
    <figure>
      <img src="../../assets/img/test2.png" alt="test" />
    </figure>
    <figure>
      <img src="../../assets/img/test3.png" alt="test" />
    </figure>
    <figure>
      <img src="../../assets/img/test4.png" alt="test" />
    </figure>
    <div class="arrows">
      <div class="prev">
        <div class="circle darker-blue">
          <img
            src="../../assets/img/image (11).svg"
            alt="prev"
            @click="changeIndex('prev')"
          />
        </div>
      </div>
      <div class="next">
        <div class="circle dark-green">
          <img
            src="../../assets/img/image (8).svg"
            alt="next"
            @click="changeIndex('next')"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
@use "../../assets/scss/variables" as *;
.testimonials-list {
  width: 100%;
  position: relative;
  background-color: #b098d4;
  figure {
    width: 25%;
    margin: 0;
    img {
      width: 100%;
      height: 400px;
    }
  }
}
.arrows {
  width: 95%;
  display: flex;
  justify-content: space-between;
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  display: flex;
  margin: 0 30px;
  .circle {
    @include center();
    @include round();
    width: 40px;
    height: 40px;
    padding: 10px;
    margin: 0 10px;
    cursor: pointer;
    img {
      filter: invert(100%) sepia(10%) saturate(2%) hue-rotate(312deg)
        brightness(112%) contrast(100%);
    }
    &.darker-blue {
      background-color: $darker-blue;
    }
    &.dark-green {
      background-color: $dark-green;
    }
    img {
      height: 18px;
    }
  }
}
</style>
