<template>
  <div class>
    <img class="splash__img" src="~/assets/img/home_splash.jpg" />
    <section class="splash">
      <div class="splash__frame">
        <div class="splash__row">
          <h2
            class="splash__text--primary type--raleway type--bold type--white type--display"
          >
            Pro-bono Corporate Finance Advisory For:
          </h2>
        </div>
        <div class="splash__row">
          <transition name="slide-fade">
            <h2
              v-if="showArray"
              class="splash__text--secondary type--raleway type--bold type--white type--display"
            >
              {{ wordArray[0] }}
            </h2>
          </transition>
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
  name: "home",
  head() {
    return {
      title: `BPC | Home`
    };
  },
  data: function() {
    return {
      wordArray: [
        "SMALL-MEDIUM BUSINESSES",
        "FAMILY BUSINESSES",
        "PROPRIETORSHIPS"
      ],
      showArray: true
    };
  },
  methods: {
    loopArray: async function(array) {
      let currentItem = array.shift();
      array.push(currentItem);
      this.showArray = !this.showArray;
    }
  },
  mounted: function() {
    setInterval(() => {
      setTimeout(() => {
        this.loopArray(this.wordArray);
      }, 200);
      this.showArray = !this.showArray;
    }, 6000);
  },
  components: {
    "footer-app": Footer
  }
};
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all 0.3s ease;
}
.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-enter,
.slide-fade-leave-to {
  transform: translateX(-5rem);
  opacity: 0;
}
</style>
