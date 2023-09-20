<script>
export default {
  name: "ArenaCard",
};
</script>

<template>
  <div class="arena-card green">
    <figure class="circle">
      <img src="../../assets/img/feature1.png" alt="feature1" />
    </figure>
    <h3>Live Streaming</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
  </div>
  <div class="arena-card blue">
    <figure class="circle">
      <img src="../../assets/img/feature2.png" alt="feature1" />
    </figure>
    <h3>Gaming News</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
  </div>
  <div class="arena-card blue">
    <figure class="circle">
      <img src="../../assets/img/feature3.png" alt="feature1" />
    </figure>
    <h3>Great Tournament</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
  </div>
  <div class="arena-card green">
    <figure class="circle">
      <img src="../../assets/img/feature4.png" alt="feature1" />
    </figure>
    <h3>Awward Ceremony</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.arena-card {
  @include center();
  width: 45%;
  height: 50%;
  border-radius: 25px;
  margin: 5px;
  flex-direction: column;
  text-align: center;
  &.green {
    background-color: $green;
    color: $darker-blue;
  }
  &.green:hover {
    background-color: $dark-blue;
    color: $white;
  }
  &.blue {
    background-color: $dark-blue;
    color: $white;
  }
  &.blue:hover {
    background-color: $green;
    color: $darker-blue;
  }
  .circle {
    @include round();
    background-color: $darker-blue;
    img {
      width: 80px;
      height: 80px;
      padding: 20px;
    }
  }
  h3 {
    font-size: 20px;
  }
  p {
    font-size: 15px;
  }
}
</style>
