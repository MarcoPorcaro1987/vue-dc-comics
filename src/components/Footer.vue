<template>
  <footer class="foot-cont">
    <div class="foot-top">
      <div class="container info-cont">
        <div class="info">
          <p>PROVA</p>
          <ul>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
          </ul>
          <p>PROVA</p>
          <ul>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
          </ul>
        </div>
        <div class="info">
          <p>PROVA</p>
          <ul>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
          </ul>
        </div>
        <div class="info">
          <p>PROVA</p>
          <ul>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
            <li><a href="#">aca</a></li>
          </ul>
        </div>
        <div class="logo-bg-cont">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="foot-bottom"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
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
</style>
