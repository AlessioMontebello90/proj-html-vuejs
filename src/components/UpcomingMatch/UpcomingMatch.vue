<script>
import MatchCard from "./MatchCard.vue";
export default {
  name: "UpcomingMatch",
  components: {
    MatchCard,
  },
};
</script>

<template>
  <div class="match-list">
    <div class="container">
      <h5>Trading Battle</h5>
      <h3>Upcoming Match</h3>
      <ul class="d-flex mx-2">
        <li>All</li>
        <li>Pubg</li>
        <li>COD</li>
        <li>AC</li>
        <li>MCX</li>
      </ul>
      <MatchCard />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
.match-list {
  padding: 150px 0;
  text-align: center;
  background-color: $darkest-blue;
  h5 {
    color: $dark-green;
    margin-bottom: 20px;
  }
  h3 {
    color: $white;
    margin-bottom: 35px;
    font-size: 50px;
  }
  ul {
    list-style-type: none;
  }
}
</style>
