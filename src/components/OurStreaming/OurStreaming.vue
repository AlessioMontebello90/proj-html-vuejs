<script>
export default {
  name: "OurStreaming",
  data() {
    return {
      index: 1,
    };
  },
  methods: {
    SetIndex() {
      if (this.index === 1) {
        this.index = 2;
      } else {
        this.index = 1;
      }
    },
  },
};
</script>

<template>
  <section class="our-streaming">
    <div class="container h-100">
      <div class="live-stream h-100">
        <figure>
          <img
            v-if="index === 1"
            class="img-fluid"
            src="../../assets/img/v-small1.png"
            alt="Call of duty"
          />
          <img
            v-else
            class="img-fluid"
            src="../../assets/img/v-small2.png"
            alt="Call of deuty"
          />
          <a class="play" href="#">
            <img
              class="img-fluid"
              src="../../assets/img/image (9).svg"
              alt="play-right"
          /></a>
        </figure>
      </div>
      <div class="all-streams">
        <div class="info d-flex">
          <div class="title">
            <h5>Live Streaming</h5>
            <h3>Checkout Our Live Streaming</h3>
          </div>
          <div class="arrows">
            <div class="prev">
              <div class="circle green">
                <img
                  src="../../assets/img/image (11).svg"
                  alt="prev"
                  @click="SetIndex"
                />
              </div>
            </div>
            <div class="next">
              <div class="circle white">
                <img
                  src="../../assets/img/image (8).svg"
                  alt="next"
                  @click="SetIndex"
                />
              </div>
            </div>
          </div>
        </div>
        <div class="streams">
          <figure>
            <img src="../../assets/img/v-small1.png" alt="call" />
            <figcaption>
              <h4>Call Of Duty</h4>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            </figcaption>
          </figure>
          <figure>
            <img src="../../assets/img/v-small2.png" alt="assassin" />
            <figcaption>
              <h4>Assassins Creed</h4>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            </figcaption>
          </figure>
        </div>
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
        width: 600px;
        height: 400px;
        position: relative;
        margin-right: 20px;
        img {
          width: 100%;
          height: 100%;
        }
      }
      a.play {
        @include center();
        @include round();
        @include absolute-center();
        text-decoration: none;
        color: $white;
        background-color: $green;
        padding: 20px 22px;

        img {
          height: 20px;
          filter: invert(100%) sepia(10%) saturate(2%) hue-rotate(312deg)
            brightness(112%) contrast(100%);
        }
      }
    }
    .all-streams {
      h5 {
        color: $dark-green;
        margin-bottom: 10px;
      }
      h3 {
        color: $white;
        margin-bottom: 35px;
        font-size: 37px;
      }
      .info {
        align-items: flex-end;
      }
      .arrows {
        display: flex;
        margin: 30px;
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
      .streams {
        display: flex;
        figure {
          img {
            height: 180px;
            margin-right: 60px;
          }
          figcaption {
            color: $white;
            margin: 5px;
          }
        }
      }
    }
  }
}
</style>
