<script>
export default {
  name: "NavbarMenu",
  data() {
    return {
      links: [
        {
          name: "HOME",
          href: "#",
          subnav: [
            {
              menuName: "About Us",
              href: "#",
            },
            {
              menuName: "Matches",
              href: "#",
            },
            {
              menuName: "Team",
              href: "#",
            },
            {
              menuName: "Squad",
              href: "#",
            },
            {
              menuName: "Squad Details",
              href: "#",
            },
            {
              menuName: "Comming Soon",
              href: "#",
            },
            {
              menuName: "404",
              href: "#",
            },
          ],
        },
        {
          name: "PAGES",
          href: "#",
          subnav: [
            {
              menuName: "About Us",
              href: "#",
            },
            {
              menuName: "Matches",
              href: "#",
            },
            {
              menuName: "Team",
              href: "#",
            },
            {
              menuName: "Squad",
              href: "#",
            },
            {
              menuName: "Squad Details",
              href: "#",
            },
            {
              menuName: "Comming Soon",
              href: "#",
            },
            {
              menuName: "404",
              href: "#",
            },
          ],
        },
        {
          name: "TOURNAMENT",
          href: "#",
        },
        {
          name: "SHOP",
          href: "#",
          subnav: [
            {
              menuName: "About Us",
              href: "#",
            },
            {
              menuName: "Matches",
              href: "#",
            },
            {
              menuName: "Team",
              href: "#",
            },
            {
              menuName: "Squad",
              href: "#",
            },
            {
              menuName: "Squad Details",
              href: "#",
            },
            {
              menuName: "Comming Soon",
              href: "#",
            },
            {
              menuName: "404",
              href: "#",
            },
          ],
        },
        {
          name: "BLOG",
          href: "#",
          subnav: [
            {
              menuName: "About Us",
              href: "#",
            },
            {
              menuName: "Matches",
              href: "#",
            },
            {
              menuName: "Team",
              href: "#",
            },
            {
              menuName: "Squad",
              href: "#",
            },
            {
              menuName: "Squad Details",
              href: "#",
            },
            {
              menuName: "Comming Soon",
              href: "#",
            },
            {
              menuName: "404",
              href: "#",
            },
          ],
        },
        {
          name: "CONTACT",
          href: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="collapse navbar-collapse" id="navbarNavDropdown">
    <ul class="navbar-nav">
      <li v-for="link in this.links" class="nav-item dropdown">
        <a
          v-if="link.subnav"
          class="nav-link dropdown-toggle"
          :href="link.href"
          data-bs-toggle="dropdown"
        >
          {{ link.name }}
        </a>
        <a v-else class="nav-link" :href="link.href">
          {{ link.name }}
        </a>
        <ul class="dropdown-menu">
          <li v-for="sub in link.subnav">
            <a class="dropdown-item" :href="sub.href">{{ sub.menuName }}</a>
          </li>
        </ul>
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
  ul {
    li {
      margin: 0 10px;
    }
    a {
      &:hover {
        color: $dark-green;
      }
      &:focus {
        color: $dark-green;
      }
    }
  }
  ul.dropdown-menu.show {
    background-color: $darker-blue;
    border-radius: 0;
    padding: 0;
    margin: 0;
    border: 0;
    min-width: 100%;
    li {
      margin: 0;
      &::after {
        content: "";
        display: block;
        margin: 0 10px;
        height: 1px;
        border-top: 1px solid $white;
      }
      &:last-of-type::after {
        border-top: 0 solid $white;
      }
    }
  }
  .dropdown-item {
    width: 100%;
    padding: 5px 10px;
    font-size: 13px;
    &:hover {
      background-color: rgba($black, 0.6);
    }
  }
  .show {
    color: $dark-green;
  }
}
</style>
