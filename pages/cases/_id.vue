<template>
  <div>
    <section class="article">
      <button
        @click="hasHistory() ? $router.go(-1) : $router.push('/')"
        type="button"
        class="article__redirect type--raleway type--body type--secondary type--underline"
      >back to previous page</button>
      <div class="article__body">
        <static-template></static-template>
      </div>
    </section>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
import Template from "@/static/cases/test";

export default {
  name: "post",
  data() {
    return {};
  },
  head() {
    return {
      title: `BPC | Case Study`,
    };
  },
  computed: {},
  methods: {
    hasHistory() {
      return window.history.length > 2;
    },
  },
  components: {
    "footer-app": Footer,
    "static-template": Template,
  },
  created() {},
};
</script>

<style></style>
