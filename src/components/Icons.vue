<template>
  <div class="icons">
    <div class="container icons-cont">
      <div class="icon" v-for="(icon, index) in icons" :key="index">
        <img :src="require(`@/assets/img/${icon.img}`)" alt="icon.label" />
        <span>{{icon.label}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Icons",
  data() {
    return {
      icons: [
        {
          img: "buy-comics-digital-comics.png",
          label: "DIGITAL COMICS",
        },
        {
          img: "buy-comics-merchandise.png",
          label: "DC MERCHANDISE",
        },
        {
          img: "buy-comics-subscriptions.png",
          label: "SUBSCRIPTION",
        },
        {
          img: "buy-comics-shop-locator.png",
          label: "COMIC SHOP LOCATOR",
        },
        {
          img: "buy-dc-power-visa.svg",
          label: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables.scss";
.icons {
  background: $mainColor;
  padding: 1.5625rem;
}
.icons-cont {
  padding: 20px;
  display: flex;
  color: white;
  justify-content: space-between;
  .icon {
    display: flex;
    align-items: center;
    gap: 1.25rem;
    span {
      font-size: 0.75rem;
    }
    img {
      height: 3.125rem;
    }
  }
}
</style>
