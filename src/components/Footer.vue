<template>
  <footer class="foot-cont">
    <div class="foot-top">
      <div class="container info-cont">
        <div class="info">
          <p>DC COMICS</p>
          <ul>
            <li v-for="(link, index) in menu1" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
          <p>SHOP</p>
          <ul>
            <li v-for="(link, index) in menu2" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="info">
          <p>DC</p>
          <ul>
            <li v-for="(link, index) in menu3" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="info">
          <p>SITES</p>
          <ul>
            <li v-for="(link, index) in menu4" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="logo-bg-cont">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="foot-bottom">
      <div class="container foot-btm-cont">
        <div class="btn-sign-up">SIGN-UP NOW!</div>
        <div class="social-cont">
          <p class="">FOLLOW US</p>
          <div class="social" v-for="(social, index) in socials" :key="index">
            <a href="social.url"
              ><img
                :src="require(`@/assets/img/${social.src}`)"
                :alt="social.text"
            /></a>
          </div>
          <img src="" alt="" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      menu1: [
        {
          text: "Characters",
          url: "#",
        },
        {
          text: "Comics",
          url: "#",
        },
        {
          text: "Movies",
          url: "#",
        },
        {
          text: "TV",
          url: "#",
        },
        {
          text: "Games",
          url: "#",
        },
        {
          text: "Videos",
          url: "#",
        },
        {
          text: "News",
          url: "#",
        },
      ],
      menu2: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC Collectibles",
          url: "#",
        },
      ],
      menu3: [
        {
          text: "Term Of Use",
          url: "#",
        },
        {
          text: "Privacy policy(New)",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "GAMES",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      menu4: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD Magazine",
          url: "#",
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
          url: "#",
        },
      ],
      socials: [
        {
          text: "Facebook",
          src: "footer-facebook.png",
          url: "#",
        },
        {
          text: "Twitter",
          src: "footer-twitter.png",
          url: "#",
        },
        {
          text: "Youtube",
          src: "footer-youtube.png",
          url: "#",
        },
        {
          text: "Pinterest",
          src: "footer-pinterest.png",
          url: "#",
        },
        {
          text: "Periscope",
          src: "footer-periscope.png",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables.scss";
.foot-top {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 21rem;
  background-size: contain;
  overflow: hidden;
}
.info-cont {
  display: flex;
  gap: 2.5rem;
}
.info {
  padding: 1.875rem 0;
  p {
    padding: 0.625rem 0;
    font-weight: bold;
    color: white;
  }
  a {
    color: #959595;
    font-size: 0.75rem;
  }
}
.logo-bg-cont {
  margin-left: auto;
  margin-top: -5%;
  img {
    height: 28.125rem;
  }
}
.foot-bottom {
  background-color: #303030;
  display: flex;
  padding: 1.25rem 0;
}
.foot-btm-cont {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
  .btn-sign-up {
    color: white;
    padding: 0.3125rem 0.625rem;
    border: 2px solid $mainColor;
  }
  p {
    color: $mainColor;
  }
  .social-cont {
    display: flex;
    align-items: center;
    gap: 0.9375rem;
  }
}
</style>
