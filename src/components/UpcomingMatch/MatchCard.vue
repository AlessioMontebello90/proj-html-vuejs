<script>
export default {
  name: "MatchCard",
  props: {
    list: Array,
  },
};
</script>

<template>
  <div
    v-if="this.list.all || this.list.Pubg"
    class="match-card mb-5 d-flex justify-content-between"
  >
    <div class="players">
      <div class="player-card d-flex">
        <figure>
          <img class="img-fluid" src="../../assets/img/t3.png" alt="ninja" />
          <figcaption>
            <h5>Italy</h5>
            <h2>Ninja Gaming</h2>
          </figcaption>
        </figure>
        <div class="vs d-flex align-items-center justify-content-center">
          VS
        </div>
        <figure>
          <img class="img-fluid" src="../../assets/img/t4.png" alt="ninja" />
          <figcaption>
            <h5>India</h5>
            <h2>Witch Gaaming</h2>
          </figcaption>
        </figure>
      </div>
    </div>
    <div class="game">
      <h2>PUBG Battleground</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci,
        temporibus officia deserunt ullam repellendus unde similique quo
      </p>
    </div>
    <div class="date">
      <h2>10.45</h2>
      <p class="m-0">1st November, 2022</p>
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
  </div>
  <div
    v-if="this.list.all || this.list.AC"
    class="match-card mb-5 d-flex justify-content-between"
  >
    <div class="players">
      <div class="player-card d-flex">
        <figure>
          <img class="img-fluid" src="../../assets/img/t1.png" alt="ninja" />
          <figcaption>
            <h5>Italy</h5>
            <h2>King Gaming</h2>
          </figcaption>
        </figure>
        <div class="vs d-flex align-items-center justify-content-center">
          VS
        </div>
        <figure>
          <img src="../../assets/img/t2.png" alt="ninja" />
          <figcaption>
            <h5>India</h5>
            <h2>Witch Astro</h2>
          </figcaption>
        </figure>
      </div>
    </div>
    <div class="game">
      <h2>Assassain's Creed</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci,
        temporibus officia deserunt ullam repellendus unde similique quo
      </p>
    </div>
    <div class="date">
      <h2>09.45</h2>
      <p class="m-0">1st November, 2022</p>
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
  </div>
  <div
    v-if="this.list.all || this.list.Mcx"
    class="match-card mb-5 d-flex justify-content-between"
  >
    <div class="players">
      <div class="player-card d-flex">
        <figure>
          <img class="img-fluid" src="../../assets/img/t5.png" alt="ninja" />
          <figcaption>
            <h5>Italy</h5>
            <h2>Dgn Gaming</h2>
          </figcaption>
        </figure>
        <div class="vs d-flex align-items-center justify-content-center">
          VS
        </div>
        <figure>
          <img class="img-fluid" src="../../assets/img/t6.png" alt="ninja" />
          <figcaption>
            <h5>India</h5>
            <h2>Jocker Gaming</h2>
          </figcaption>
        </figure>
      </div>
    </div>
    <div class="game">
      <h2>Mortal Combat X</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci,
        temporibus officia deserunt ullam repellendus unde similique quo
      </p>
    </div>
    <div class="date">
      <h2>08.45</h2>
      <p class="m-0">1st November, 2022</p>
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
  </div>
  <div
    v-if="this.list.all || this.list.Cod"
    class="match-card mb-5 d-flex justify-content-between"
  >
    <div class="players">
      <div class="player-card d-flex">
        <figure>
          <img class="img-fluid" src="../../assets/img/t7.png" alt="ninja" />
          <figcaption>
            <h5>Italy</h5>
            <h2>Shark Gaaming</h2>
          </figcaption>
        </figure>
        <div class="vs d-flex align-items-center justify-content-center">
          VS
        </div>
        <figure>
          <img class="img-fluid" src="../../assets/img/t8.png" alt="ninja" />
          <figcaption>
            <h5>India</h5>
            <h2>Krull Gaaming</h2>
          </figcaption>
        </figure>
      </div>
    </div>
    <div class="game">
      <h2>Call Of Deauty</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci,
        temporibus officia deserunt ullam repellendus unde similique quo
      </p>
    </div>
    <div class="date">
      <h2>04.45</h2>
      <p class="m-0">1st November, 2022</p>
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
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.match-card {
  width: 100%;
  height: 300px;
  background-color: $dark-blue;
  padding: 10px;
  border-radius: 25px;
  align-items: center;
  &:hover {
    background-color: $blue;
  }
  &:hover .date {
    background-color: $green;
    color: $black;
    .circle {
      background-color: $darkest-blue;
      img {
        filter: invert(100%) sepia(10%) saturate(2%) hue-rotate(312deg)
          brightness(112%) contrast(100%);
      }
    }
  }
  .player-card {
    height: 100%;
    align-items: center;
    figure {
      background-color: $darkest-blue;
      margin: 0 10px;
      border-radius: 25px;
      figcaption {
        padding: 5px;
        background-color: $darker-blue;
        border-bottom-left-radius: 25px;
        border-bottom-right-radius: 25px;
        h5 {
          color: $dark-green;
        }
        h2 {
          color: $white;
          font-size: 25px;
        }
      }
    }
    .vs {
      color: $dark-green;
      border-radius: 25px;
      background-color: $darkest-blue;
      width: 100px;
      height: 100px;
    }
  }
  .game {
    width: 30%;
    text-align: start;
    margin: 0 20px;
    color: $white;
  }
  .date {
    background-color: $darkest-blue;
    color: $white;
    border-radius: 25px;
    padding: 5px;
    margin: 0 15px;
    width: 130px;
    height: 130px;
    .circle {
      @include center();
      width: 25px;
      height: 25px;
      border-radius: 50%;
      padding: 7px;
      margin: 0 5px;
      background-color: $green;
    }
  }
}
</style>
