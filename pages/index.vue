<template>
  <div class>
    <img class="splash__img" src="~/assets/img/home_splash.jpg" />
    <section class="splash">
      <div class="splash__frame">
        <div class="splash__row">
          <h2
            class="splash__text--primary type--raleway type--bold type--white type--display"
          >Pro-bono Corporate Finance Advisory For:</h2>
        </div>
        <div class="splash__row">
          <h2
            class="splash__text--secondary type--raleway type--bold type--white type--display"
          >SMBs</h2>
          <div class="window__splash"></div>
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
      title: `BPC | Home`,
    };
  },
  components: {
    "footer-app": Footer,
  },
};
</script>

<style></style>
