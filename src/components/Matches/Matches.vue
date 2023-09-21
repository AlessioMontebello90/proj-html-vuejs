<script>
import MatchesCard from "./MatchesCard.vue";
export default {
  name: "Matches",
  components: {
    MatchesCard,
  },
};
</script>

<template>
  <div class="matches">
    <div class="container">
      <div class="title d-flex justify-content-between align-items-end">
        <div class="text">
          <h5>Trading Battle</h5>
          <h3 class="m-0">Upcoming Match</h3>
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
      <MatchesCard />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.matches {
  @include center("cross");
  height: 100vh;
  background-image: url("../../assets/img/v-bg.png");
  padding: 150px 0;
}
h5 {
  width: 130px;
  color: $dark-green;
  background-color: rgba($black, 0.2);
}
h3 {
  color: $white;
  font-size: 40px;
}
.circle {
  @include center();
  width: 25px;
  height: 25px;
  border-radius: 50%;
  padding: 7px;
  margin: 0 5px;
  background-color: $green;
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
