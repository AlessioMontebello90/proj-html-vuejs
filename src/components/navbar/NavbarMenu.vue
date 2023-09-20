<script>
export default {
  name: "NavbarMenu",
  data() {
    return {
      links: {
        home: {
          sublink1: "Home",
          sublink2: "Restart",
          sublink3: "Go Back",
          sublink4: "Homepage",
        },
        pages: {
          sublink1: "PAGES",
          sublink2: "About Us",
          sublink3: "Matches",
          sublink4: "Team",
          sublink5: "Squad ",
          sublink6: "Squad Details",
          sublink7: "Comming Soon",
          sublink8: "404",
        },
      },
    };
  },
};
</script>

<template>
  <div class="collapse navbar-collapse" id="navbarNavDropdown">
    <ul class="navbar-nav">
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" data-bs-toggle="dropdown">
          HOME
        </a>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">HOME</a></li>
          <li><a class="dropdown-item" href="#">HOME</a></li>
          <li><a class="dropdown-item" href="#">HOME</a></li>
        </ul>
      </li>
      <li class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          PAGES
        </a>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">PAGES</a></li>
          <li><a class="dropdown-item" href="#">PAGES</a></li>
          <li><a class="dropdown-item" href="#">PAGES</a></li>
        </ul>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">TOURNAMENT</a>
      </li>
      <li class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          SHOP
        </a>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">SHOP</a></li>
          <li><a class="dropdown-item" href="#">SHOP</a></li>
          <li><a class="dropdown-item" href="#">SHOP</a></li>
        </ul>
      </li>
      <li class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          BLOG
        </a>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">BLOG</a></li>
          <li><a class="dropdown-item" href="#">BLOG</a></li>
          <li><a class="dropdown-item" href="#">BLOG</a></li>
        </ul>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">CONTACT</a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
a {
  padding: 5px;
  color: $white;
}
#navbarNavDropdown {
  justify-content: center;
  a {
    &:hover {
      color: #05cc7c;
    }
  }
  ul.dropdown-menu.show {
    background-color: transparent;
    padding: 5px 10px;
    border: 0;
    min-width: 100%;
  }
  .dropdown-item {
    &:hover {
      background-color: rgba($black, 0.6);
    }
    padding: 3px 0;
  }
  .show {
    color: $dark-green;
  }
}
</style>
