<script>
import Logo from "./Logo.vue";
export default {
  name: "AppFooter",
  data() {
    return {
      links: [
        {
          name: "HOME",
          href: "#",
        },
        {
          name: "PAGES",
          href: "#",
        },
        {
          name: "TOURNAMENT",
          href: "#",
        },
        {
          name: "SHOP",
          href: "#",
        },
        {
          name: "BLOG",
          href: "#",
        },
        {
          name: "CONTACT",
          href: "#",
        },
      ],
    };
  },
  components: {
    Logo,
  },
};
</script>
<template>
  <footer>
    <div class="container">
      <div id="links">
        <div class="d-flex justify-content-between align-items-center">
          <Logo />
          <ul class="d-flex">
            <li v-for="link in links">
              <a :href="link.href">{{ link.name }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div
        class="copyright-social d-flex justify-content-between align-items-center"
      >
        <div class="copyright">
          <p>Copyright RaxG | Designed by <a href="#">NextGenerationDev</a></p>
        </div>
        <div
          class="social-links d-flex justify-content-between align-items-center"
        >
          <figure>
            <img
              class="img-fluid"
              src="../assets/img/image (4).svg"
              alt="facebook"
            />
          </figure>
          <figure>
            <img
              class="img-fluid"
              src="../assets/img/image (5).svg"
              alt="twitter"
            />
          </figure>
          <figure>
            <img
              class="img-fluid"
              src="../assets/img/image (6).svg"
              alt="linkedin"
            />
          </figure>
          <figure>
            <img
              class="img-fluid"
              src="../assets/img/image (7).svg"
              alt="instagram"
            />
          </figure>
        </div>
      </div>
    </div>
  </footer>
</template>
<style scoped lang="scss">
@use "../assets/scss/variables" as *;
@use "../assets/scss/mixins" as *;
footer {
  height: 50vh;
  background-image: url("../assets/img/banner1.png");
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: flex-end;
  #links {
    &::after {
      content: "";
      display: block;
      width: 100%;
      margin-bottom: 20px;
      height: 1px;
      border-top: 1px solid $white;
    }
    ul {
      list-style-type: none;
      li {
        margin: 0 5px;
        a {
          color: white;
          text-decoration: none;
          font-size: 15px;
        }
      }
    }
  }
  .copyright {
    p {
      color: $white;
      a {
        color: $dark-green;
        text-decoration: none;
      }
    }
  }
}
.social-links {
  figure {
    @include center();
    @include round();
    width: 50px;
    height: 50px;
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
</style>
