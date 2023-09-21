<script>
export default {
  name: "OurExpertsCard",
};
</script>

<template>
  <div class="experts-list d-flex justify-content-center">
    <div class="experts-card my-5">
      <figure>
        <img class="img-fluid" src="../../assets/img/team1.png" alt="team" />
        <div class="social-links justify-content-between align-items-center">
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
        <figcaption class="d-flex justify-content-center align-items-center">
          <div class="text">
            <h6>Cristiano Messi</h6>
            <p>CEO/Founder</p>
          </div>
        </figcaption>
      </figure>
    </div>
    <div class="experts-card my-5">
      <figure>
        <img class="img-fluid" src="../../assets/img/team2.png" alt="team" />
        <div class="social-links justify-content-between align-items-center">
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
        <figcaption class="d-flex justify-content-center align-items-center">
          <div class="text">
            <h6>Sergio Naymer</h6>
            <p>Programmer</p>
          </div>
        </figcaption>
      </figure>
    </div>
    <div class="experts-card my-5">
      <figure>
        <img class="img-fluid" src="../../assets/img/team3.png" alt="team" />
        <div class="social-links justify-content-between align-items-center">
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
        <figcaption class="d-flex justify-content-center align-items-center">
          <div class="text">
            <h6>Antonela Roccuzzo</h6>
            <p>Project Manager</p>
          </div>
        </figcaption>
      </figure>
    </div>
    <div class="experts-card my-5">
      <figure>
        <img class="img-fluid" src="../../assets/img/team4.png" alt="team" />
        <div class="social-links justify-content-between align-items-center">
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
        <figcaption class="d-flex justify-content-center align-items-center">
          <div class="text">
            <h6>Lionel Ramos</h6>
            <p>Game Designer</p>
          </div>
        </figcaption>
      </figure>
    </div>
  </div>
</template>

<style scss lang="scss">
@use "../../assets/scss/mixins" as *;
@use "../../assets/scss/variables" as *;
.experts-card {
  margin: 0 20px;
  position: relative;
  &:hover figcaption {
    background-color: $green;
    color: $darker-blue;
  }
  &:hover figure {
    .social-links {
      display: flex;
    }
  }
  figure {
    width: 200px;
    .social-links {
      display: none;
      position: absolute;
      left: 50%;
      bottom: 90px;
      transform: translate(-50%);
      figure {
        @include center();
        @include round();
        width: 30px;
        height: 30px;
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
  }
  figcaption {
    width: 200px;
    height: 80px;
    color: $white;
    text-align: center;
    background-color: $darker-blue;
    h6 {
      font-size: 18px;
    }
    p {
      font-size: 12px;
    }
  }
}
</style>
