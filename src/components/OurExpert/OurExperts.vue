<script>
import OurExpertsCard from "./OurExpertsCard.vue";
export default {
  name: "OurExperts",
  components: {
    OurExpertsCard,
  },
};
</script>

<template>
  <div class="our-experts">
    <div class="container">
      <div class="title d-flex justify-content-between align-items-end">
        <div class="text">
          <h5>Team Members</h5>
          <h3 class="m-0">Our Experts Team Members</h3>
        </div>
        <div class="arrows">
          <div class="prev">
            <div class="circle green">
              <img
                src="../../assets/img/image (11).svg"
                alt="prev"
                @click="changeIndex('prev')"
              />
            </div>
          </div>
          <div class="next">
            <div class="circle white">
              <img
                src="../../assets/img/image (8).svg"
                alt="next"
                @click="changeIndex('next')"
              />
            </div>
          </div>
        </div>
      </div>
      <OurExpertsCard />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
@use "../../assets/scss/variables" as *;
.our-experts {
  height: 90vh;
  background-color: $darkest-blue;
  padding: 150px 0;
}
h5 {
  color: $dark-green;
}
h3 {
  color: $white;
  font-size: 40px;
}
.arrows {
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
    &.green {
      background-color: $green;
      img {
        filter: invert(100%) sepia(10%) saturate(2%) hue-rotate(312deg)
          brightness(112%) contrast(100%);
      }
    }
    &.white {
      background-color: $white;
    }
    img {
      height: 18px;
    }
  }
}
</style>
