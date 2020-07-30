<template>
  <div>
    <div class="about">
      <submenu-app :menu-items="menuItems"></submenu-app>
      <div class="leadership-container">
        <div class="leadership-header">
          <h2
            class="leadership-header__heading type--raleway type--heading type--secondary"
          >Justin Ulster</h2>
          <h3 class="type--raleway type--subheading type--thin type--grey-dark">Managing Director</h3>
        </div>
        <div class="leadership-links">
          <a
            href="mailto:mail@mail.com"
            class="leadership-links__link type--raleway type--body type--secondary type--underline"
          >mail@mail.com</a>
          <p class="leadership-links__divider">|</p>
          <a
            href="tel:+4162708568"
            class="leadership-links__link type--raleway type--body type--secondary type--underline"
          >+1 (416) 270-8568</a>
        </div>
        <p class="type--open-sans type--body type--primary">
          Justin
          Ulster founded the firm in 2020 with the intention of serving small to medium size family owned businesses. Justin serves as
          the Managing Partner of the firm, providing advisory and valuation services to clients, while overseeing the corporate direction and
          initiatives of BP&Co Justin has extensive experience working across a variety of transactions including equity and debt underwriting,
          and M&A advisory He holds an Honours Business Administration degree from Wilfrid Laurier University
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
  name: "leadership",
  head() {
    return {
      title: `BPC | Leadership`,
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