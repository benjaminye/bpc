<template>
  <div>
    <div class="cases-page">
      <section class="featured">
        <img class="featured__img" src="~/assets/img/case_featured.jpg" alt="inkdrop" />
        <div class="featured__section">
          <div class="featured__section-header">
            <h1
              class="featured__section-header-heading type--raleway type--bold type--white type--xlarge"
            >FEATURED CASE STUDY</h1>
            <h2
              class="featured__section-header-subheading type--raleway type--medium type--subheading type--champaigne"
            >Equity | Technology</h2>
          </div>
          <div class="featured__section-article">
            <h1
              class="featured__section-article-heading type--libre-franklin type--bold type--large type--white"
            >Project Something</h1>
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

      <div class="cases-content">
        <article-list-app :article-items="articleItems"></article-list-app>
      </div>
    </div>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
import ArticleList from "@/components/ArticleList";

import articleItems from "@/static/store/articles-cases.json";

export default {
  name: "cases",
  head() {
    return {
      title: `BPC | Case Studies`,
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