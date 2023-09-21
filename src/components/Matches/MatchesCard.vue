<script>
import LinkButton from "../Buttons/LinkButton.vue";
export default {
  name: "MatchesCard",
  components: {
    LinkButton,
  },
  data() {
    return {
      text: "View",
    };
  },
};
</script>

<template>
  <div class="matches-list d-flex justify-content-around">
    <div class="matches-card">
      <figure>
        <img src="../../assets/img/1.png" alt="ninja" />
        <figcaption>
          <h3>Ninja Warrior Gaming</h3>
          <div class="links">
            <div class="links d-flex justify-content-center">
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (13).svg"
                  alt="youtube"
                />
              </div>
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (14).svg"
                  alt="chat"
                />
              </div>
            </div>
          </div>
          <h2 class="m-2">9.45</h2>
          <p>1st November, 2022</p>
          <LinkButton :text="text" />
        </figcaption>
      </figure>
    </div>
    <div class="matches-card">
      <figure>
        <img src="../../assets/img/5.png" alt="ninja" />
        <figcaption>
          <h3>Witch Gaming</h3>
          <div class="links">
            <div class="links d-flex justify-content-center">
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (13).svg"
                  alt="youtube"
                />
              </div>
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (14).svg"
                  alt="chat"
                />
              </div>
            </div>
          </div>
          <h2 class="m-2">9.45</h2>
          <p>1st November, 2022</p>
          <LinkButton :text="text" />
        </figcaption>
      </figure>
    </div>
    <div class="matches-card">
      <figure>
        <img src="../../assets/img/3.png" alt="ninja" />
        <figcaption>
          <h3>SkullG Gaming</h3>
          <div class="links">
            <div class="links d-flex justify-content-center">
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (13).svg"
                  alt="youtube"
                />
              </div>
              <div class="circle">
                <img
                  class="img-fluid"
                  src="../../assets/img/image (14).svg"
                  alt="chat"
                />
              </div>
            </div>
          </div>
          <h2 class="m-2">9.45</h2>
          <p>1st November, 2022</p>
          <LinkButton :text="text" />
        </figcaption>
      </figure>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.matches-card {
  @include center("main");
  border-radius: 25px;
  width: 300px;
  height: 450px;
  background-color: $darker-blue;
  padding: 30px 0;
  margin: 50px 0;
  figure {
    border-radius: 25px;
    text-align: center;
    width: 80%;
    height: 180px;
    background-color: $darkest-blue;
    position: relative;
    figcaption {
      padding: 30px 0;
      color: $white;
    }
  }
}
h3 {
  font-size: 22px;
  margin: 15px 0;
}
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
.circle {
  @include center();
  width: 25px;
  height: 25px;
  border-radius: 50%;
  padding: 7px;
  margin: 0 5px;
  background-color: $green;
}
</style>
