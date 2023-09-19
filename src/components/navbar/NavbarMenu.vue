<script>
export default {
  name: "NavbarMenu",
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
      <li class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          href="#"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          TOURNAMENT
        </a>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">TOURNAMENT</a></li>
          <li><a class="dropdown-item" href="#">TOURNAMENT</a></li>
          <li><a class="dropdown-item" href="#">TOURNAMENT</a></li>
        </ul>
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
a {
  padding: 5px;
  color: white;
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
      background-color: rgba(black, 0.6);
    }
    padding: 3px 0;
  }
  .show {
    color: #05cc7c;
  }
}
</style>
