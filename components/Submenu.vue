<template>
  <div class="submenu">
    <div v-for="(item, index) in menuItems" :key="index" class="submenu__item">
      <nuxt-link
        :to="item.to"
        class="submenu__link type--raleway type--large type--bold type--grey-dark type--underline"
      >
        {{item.title}}
        <div class="window__submenu"></div>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: ["menuItems"],
};
</script>

<style scoped lang="scss">
@import "../assets/css/abstracts/variables";
.nuxt-link-exact-active {
  color: $color-primary;
}
</style>