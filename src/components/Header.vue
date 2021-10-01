<template>
  <header class="container head-cont">
    <div class="head-left">
      <div class="logo-cont">
        <img src="../assets/img/dc-logo.png" alt="Logo DC" />
      </div>
    </div>
    <div class="head-right">
      <nav>
        <ul>
          <li v-for="(link, index) in menu" :key="index">
            <a :href="link.url" :class="{ active: link.current }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      menu: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: true,
        },
        {
          text: "MOVIES",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIBILES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.head-cont {
  display: flex;
  justify-content: space-between;
  height: 5.5rem;
  padding-top: 0.625rem;
  align-items: center;
  .head-left {
    img {
      height: 4rem;
    }
  }
  .head-right {
    ul {
      display: flex;
      gap: 2rem;
      li {
        a {
          color: #464646;
          font-size: 0.75rem;
          font-weight: 700;
          display: inline-block;
          padding: 1.875rem 0;
          &.active {
            color: $mainColor;
            border-bottom: 0.25rem solid $mainColor;
          }
        }
      }
    }
  }
}
</style>
