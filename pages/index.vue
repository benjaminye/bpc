<template>
  <div class>
    <section class="splash">
      <img class="splash__img" src="~/assets/img/home_splash.jpg" />
      <div class="splash__frame">
        <div class="splash__row">
          <h2 class="splash__text--primary splash-text">Pro-bono Corporate Finance Advisory For:</h2>
        </div>
        <div class="splash__row">
          <h2 class="splash__text--secondary splash-text">SMBs</h2>
          <div class="splash__window">
            <div class="window"></div>
          </div>
        </div>
      </div>
    </section>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";

export default {
  name: "Home",
  head() {
    return {
      title: `Bellwood Partners | ${this.$options.name}`,
    };
  },
  components: {
    "footer-app": Footer,
  },
};
</script>

<style>
</style>
