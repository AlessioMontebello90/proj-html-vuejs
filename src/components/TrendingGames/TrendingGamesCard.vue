<script>
import PlayButton from "../Buttons/PlayButton.vue";
export default {
  name: "TrendingGamesCard",
  components: {
    PlayButton,
  },
};
</script>

<template>
  <div class="cards-list d-flex justify-content-between">
    <figure>
      <div class="new">New</div>
      <img class="img-fluid" src="../../assets/img/protfolio1.png" alt="ac" />
      <figcaption class="d-flex">
        <div class="text">
          <h6>Assassin's Creed</h6>
          <p>Donce sollicitudin malesuada.</p>
        </div>
        <a class="arrow" href="#">
          <img
            class="img-fluid"
            src="../../assets/img/image (9).svg"
            alt="arrow-right"
        /></a>
      </figcaption>
    </figure>
    <figure>
      <div class="new">New</div>
      <img class="img-fluid" src="../../assets/img/protfolio2.png" alt="ac" />
      <figcaption class="d-flex">
        <div class="text">
          <h6>Call Of Deauty</h6>
          <p>Donce sollicitudin malesuada.</p>
        </div>
        <a class="arrow" href="#">
          <img
            class="img-fluid"
            src="../../assets/img/image (9).svg"
            alt="arrow-right"
        /></a>
      </figcaption>
    </figure>
    <figure>
      <div class="new">New</div>
      <img class="img-fluid" src="../../assets/img/protfolio3.png" alt="ac" />
      <figcaption class="d-flex">
        <div class="text">
          <h6>Tomb Raider</h6>
          <p>Donce sollicitudin malesuada.</p>
        </div>
        <a class="arrow" href="#">
          <img
            class="img-fluid"
            src="../../assets/img/image (9).svg"
            alt="arrow-right"
        /></a>
      </figcaption>
    </figure>
    <figure>
      <div class="new">New</div>
      <img class="img-fluid" src="../../assets/img/protfolio4.png" alt="ac" />
      <figcaption class="d-flex">
        <div class="text">
          <h6>Mortal Combat X</h6>
          <p>Donce sollicitudin malesuada.</p>
        </div>
        <a class="arrow" href="#">
          <img
            class="img-fluid"
            src="../../assets/img/image (9).svg"
            alt="arrow-right"
        /></a>
      </figcaption>
    </figure>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
figure {
  height: 250px;
  width: 250px;
  position: relative;
  &:hover figcaption {
    background-color: $green;
  }
  &:hover a.arrow {
    background-color: $darkest-blue;
    img {
      filter: invert(74%) sepia(63%) saturate(6976%) hue-rotate(125deg)
        brightness(109%) contrast(96%);
    }
  }
  .new {
    background-color: $green;
    padding: 0 5px;
    position: absolute;
    top: 0;
    left: 0;
  }
  figcaption {
    height: 70px;
    color: $white;
    background-color: $dark-blue;
    padding: 5px;
    .text {
      margin-right: 20px;
      padding-top: 10px;
      h6 {
        font-size: 16px;
      }
      p {
        font-size: 12px;
      }
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
