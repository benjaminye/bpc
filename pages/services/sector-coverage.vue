<template>
  <div>
    <div class="services">
      <submenu-app :menu-items="menuItems"></submenu-app>
      <divider-app>Our Expertise</divider-app>
      <grid-app :grid-items="gridItems"></grid-app>
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
import gridItems from "~/static/store/grid-sector.json";

export default {
  name: "sectors",
  head() {
    return {
      title: `BPC | Sector Coverage`,
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