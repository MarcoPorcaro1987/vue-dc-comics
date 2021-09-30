<template>
  <div class="book">
    <img :src="bk.thumb" :alt="bk.series" />
    <p>{{ bk.series }}</p>
  </div>
</template>

<script>
export default {
  name: "Book",
  props: ["bk"],
};
</script>

<style lang="scss" scoped>
.book {
  width: calc(100% / 6 - 2rem);
  height: 7.308125rem;
  margin-bottom: 1.875rem;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
  p {
    color: white;
    font-size: 0.875rem;
    margin-top: 0.625rem;
  }
}
</style>
