<script>
import TrendingGamesCard from "./TrendingGamesCard.vue";
export default {
  name: "TrendingGames",
  data() {
    return {
      index: 0,
    };
  },
  components: {
    TrendingGamesCard,
  },
};
</script>

<template>
  <div class="trending-games">
    <div class="container">
      <div class="choose-game d-flex justify-content-between align-items-end">
        <div class="title">
          <h5>Trending Games</h5>
          <h3 class="m-0">Choose Who Is The Best In The World!</h3>
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
      <TrendingGamesCard />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
@use "../../assets/scss/variables" as *;
.trending-games {
  background-color: $darker-blue;
  padding: 150px 0;
  .choose-game {
    margin-bottom: 30px;
  }
}
h5 {
  color: $dark-green;
  margin-bottom: 10px;
}
h3 {
  color: $white;
  margin-bottom: 35px;
  font-size: 37px;
}
.arrows {
  display: flex;
  margin: 0 30px;
  .circle {
    @include center();
    @include round();
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
