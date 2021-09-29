<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Icons />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Icons from "@/components/Icons.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Icons,
    Footer,
  },
};
</script>

<style lang="scss">
@import "@/assets/style/common";
</style>
