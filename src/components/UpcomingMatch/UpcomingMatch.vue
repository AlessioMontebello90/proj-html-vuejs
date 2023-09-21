<script>
import MatchCard from "./MatchCard.vue";
export default {
  name: "UpcomingMatch",
  components: {
    MatchCard,
  },
  data() {
    return {
      list: [
        {
          all: true,
          Pubg: true,
          Cod: true,
          AC: true,
          Mcx: true,
        },
      ],
    };
  },
  methods: {
    sort(game) {
      this.list.all = false;
      this.list.Pubg = false;
      this.list.Cod = false;
      this.list.AC = false;
      this.list.Mcx = false;
      if (game === "all") {
        this.list.all = true;
      } else if (game === "pubg") {
        this.list.Pubg = true;
      } else if (game === "cod") {
        this.list.Cod = true;
      } else if (game === "ac") {
        this.list.AC = true;
      } else if (game === "mcx") {
        this.list.Mcx = true;
      }
      console.log(this.list);
    },
  },
};
</script>

<template>
  <div class="match-list">
    <div class="container">
      <h5>Trading Battle</h5>
      <h3>Upcoming Match</h3>
      <ul class="d-flex justify-content-center mx-2">
        <li @click="sort('all')">All</li>
        <li @click="sort('pubg')">Pubg</li>
        <li @click="sort('cod')">COD</li>
        <li @click="sort('ac')">AC</li>
        <li @click="sort('mcx')">MCX</li>
      </ul>
      <MatchCard :list="list" />
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
    li {
      color: $white;
      margin: 0 10px;
      &:hover {
        color: $dark-green;
      }
    }
  }
}
</style>
