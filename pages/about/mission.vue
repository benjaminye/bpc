<template>
  <div>
    <div class="about">
      <submenu-app :menu-items="menuItems"></submenu-app>
      <div class="mission-container">
        <h2 class="mission-heading type--raleway type--heading type--secondary">Our Mission</h2>
        <p class="mission-text type--open-sans type--body type--primary">
          We help our clients within the under-served SMB environment achieve superior
          outcomes by providing thoughtful, analytical and caring advice historically provided
          solely to large enterprises. We strive to maintain an intellectually stimulating and
          collaborative work environment structured around meritocracy.
        </p>
      </div>
      <div class="mission-container">
        <h2 class="mission-heading type--raleway type--heading type--secondary">Our Vision</h2>
        <p class="type--open-sans type--body type--primary">
          We seek to be recognized as the leading independent financial advisory firm for
          small-to-medium businesses, providing preeminent strategic direction to our clients.
        </p>
      </div>
    </div>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
import Submenu from "@/components/Submenu";

import menuItems from "~/static/store/menu-about.json";

export default {
  name: "mission",
  head() {
    return {
      title: `BPC | Mission`,
    };
  },
  data: function () {
    return {
      menuItems,
    };
  },
  components: {
    "footer-app": Footer,
    "submenu-app": Submenu,
  },
};
</script>

<style>
</style>