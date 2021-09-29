<template>
  <div class="icons">
    <div class="container icons-cont">
      <div class="icon" v-for="(icon, index) in icons" :key="index">
        <img
          src="@/assets/img/buy-comics-digital-comics.png"
          alt="icons.label"
        />
        <span>PROVA</span>
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
          img: "@/assets/img/buy-comics-digital-comics.png",
          label: "DIGITAL COMICS",
        },
        {
          img: "@/assets/img/buy-comics-merchandise.png",
          label: "DC MERCHANDISE",
        },
        {
          img: "@/assets/img/buy-comics-subscriptions.png",
          label: "SUBSCRIPTION",
        },
        {
          img: "@/assets/img/buy-comics-shop-locator.png",
          label: "COMIC SHOP LOCATOR",
        },
        {
          img: "@/assets/img/buy-dc-power-visa.png",
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
