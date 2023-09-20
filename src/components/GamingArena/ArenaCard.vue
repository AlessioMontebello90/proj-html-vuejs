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
.arena-card {
  width: 45%;
  height: 50%;
  border-radius: 25px;
  margin: 5px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  &.green {
    background-color: #05cc7c;
    color: #202046;
  }
  &.blue {
    background-color: #333287;
    color: white;
  }
  .circle {
    border-radius: 50%;
    background-color: #202046;
    img {
      width: 80px;
      height: 78px;
      padding: 10px;
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
