<template>
  <div>
    <div class="services">
      <submenu-app :menu-items="menuItems"></submenu-app>
      <divider-app>Our Expertise</divider-app>
      <transition name="fade">
        <grid-app :grid-items="gridItems"></grid-app>
      </transition>
    </div>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
import Submenu from "@/components/Submenu";
import SectionDivider from "@/components/SectionDivider";
import Grid from "@/components/Grid";

import menuItems from "~/static/store/menu-services.json";
import gridItems from "~/static/store/grid-capraise.json";

export default {
  name: "capraise",
  head() {
    return {
      title: `BPC | Capital Raising Advisory`,
    };
  },
  data: function () {
    return {
      menuItems,
      gridItems,
    };
  },
  components: {
    "footer-app": Footer,
    "submenu-app": Submenu,
    "divider-app": SectionDivider,
    "grid-app": Grid,
  },
};
</script>

<style>
</style>