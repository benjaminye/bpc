<template>
  <div>
    <div class="insights-page">
      <section class="featured">
        <img class="featured__img" src="~/assets/img/insights_featured.jpg" alt="inkdrop" />
        <div class="featured__section">
          <div class="featured__section-header">
            <h1
              class="featured__section-header-heading type--raleway type--bold type--white type--xlarge"
            >Blog Post #3</h1>
            <h2
              class="featured__section-header-subheading type--raleway type--medium type--subheading type--champaigne"
            >July 25, 2020</h2>
          </div>
          <div class="featured__section-article">
            <div class="featured__article-panel">
              <p
                class="featured__section-article-text type--open-sans type--medium type--body type--white"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lectus faucibus tempor posuere urna vulputate vitae nibh turpis magna. Volutpat, tellus nunc dignissim ullamcorper viverra. Ridiculus enim sed duis nam nec. Mauris amet, aliquet et, enim vulputate lacus, odio at.</p>
              <a
                href="#"
                class="featured__section-article-btn btn-primary type--libre-franklin type--bold type--small type--white"
              >Read More</a>
            </div>
          </div>
        </div>
      </section>

      <div class="insights-content">
        <article-list-app :article-items="articleItems"></article-list-app>
      </div>
    </div>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
import ArticleList from "@/components/ArticleList";

import articleItems from "@/static/store/articles-blogs.json";

export default {
  name: "insights",
  head() {
    return {
      title: `BPC | Insights`,
    };
  },
  data: function () {
    return {
      articleItems,
    };
  },
  components: {
    "footer-app": Footer,
    "article-list-app": ArticleList,
  },
};
</script>

<style>
</style>