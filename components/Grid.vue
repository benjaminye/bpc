<template>
  <div class="grid__container">
    <div v-for="(item, index) in gridItems" :key="index" class="grid__item">
      <h2 class="grid__item-heading type--raleway type--heading type--secondary">{{item.heading}}</h2>
      <p class="grid__item-body type--open-sans type--body type--primary">{{item.body}}</p>
      <nuxt-link
        v-if="!isLinkNull(item.link)"
        :to="item.link"
        class="type--raleway type--body type--secondary type--underline"
      >read case study</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: ["gridItems"],
  methods: {
    isLinkNull(link) {
      return link == null;
    },
  },
};
</script>

<style>
</style>