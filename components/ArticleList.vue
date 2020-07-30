<template>
  <section class="article-list">
    <div class="search">
      <p class="search__prompt type--raleway type--subheading type--primary">Keyword</p>
      <img src="~/assets/img/search-icon.svg" alt="Search icon" class="search__icon" />
      <input
        type="text"
        class="search__input type--open-sans type--body type--primary"
        v-model="searchText"
      />
    </div>
    <div v-for="(article, index) in filteredArticle" :key="index" class="article-box">
      <nuxt-link
        :to="article.to"
        class="article-box__heading type--raleway type--heading type--secondary type--bold"
      >{{article.title}}</nuxt-link>
      <p class="article-box__body type--open-sans type--body type--primary">{{article.subtitle}}</p>
      <p
        class="article-box__info type--raleway type--body type--grey-dark-2"
      >Tags: {{tagsString(article.tags)}}</p>
    </div>
  </section>
</template>

<script>
export default {
  props: ["articleItems"],
  data: function () {
    return {
      searchText: "",
    };
  },
  methods: {
    tagsString: function (tags) {
      return tags.join(", ");
    },
    arrayToLower: function (array) {
      return array.map((value) => value.toLowerCase());
    },
  },
  computed: {
    filteredArticle() {
      let search = this.searchText.toLowerCase();
      if (this.searchText == "") {
        return this.articleItems;
      }
      return this.articleItems.filter((article) => {
        return (
          article.title.toLowerCase().includes(search) ||
          article.subtitle.toLowerCase().includes(search) ||
          this.arrayToLower(article.tags).includes(search) ||
          this.arrayToLower(article.keywords).includes(search)
        );
      });
    },
  },
};
</script>

<style>
</style>