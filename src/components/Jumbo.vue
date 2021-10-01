<template>
  <div class="jumbo-cont" :style="`background-image: url(${bgImage})`">
    <div class="btn-current-series">{{ btn }}</div>
  </div>
</template>

<script>
export default {
  name: "Jumbo",
  props: ["bgImage", "btn"],
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.jumbo-cont {
  height: 25rem;
  background-size: cover;
  position: relative;
  .btn-current-series {
    background-color: $mainColor;
    padding: 0.625rem;
    color: white;
    display: inline-block;
    position: absolute;
    bottom: -1.275rem;
    left: 17%;
  }
}
</style>
