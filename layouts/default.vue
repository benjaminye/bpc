<template>
  <div>
    <nav class="nav">
      <header class="header">
        <nuxt-link to="/" class="header__link">
          <img
            src="~/assets/img/logo-light.svg"
            alt="Bellwood Partners Logo"
            class="header__logo-img"
          />
          <h1 class="header__logo-text type-logo--large">
            Bellwood
            <br />Partners & Co
          </h1>
        </nuxt-link>
      </header>
      <div class="menu">
        <div class="menu__column">
          <nuxt-link
            to="/services/strategic-advisory"
            class="menu__column-item type--philosopher type--white type--heading"
          >Services</nuxt-link>
          <hr class="menu__column-divider" />
          <nuxt-link
            to="/cases"
            class="menu__column-item type--philosopher type--white type--heading"
          >Case Studies</nuxt-link>
        </div>
        <div class="menu__column">
          <nuxt-link
            to="/insights"
            class="menu__column-item type--philosopher type--white type--heading"
          >Insights</nuxt-link>
          <hr class="menu__column-divider" />
          <nuxt-link
            to="/about/mission"
            class="menu__column-item type--philosopher type--white type--heading"
          >About</nuxt-link>
        </div>
        <div class="menu__column">
          <nuxt-link
            to="/contact"
            class="menu__button btn-primary btn-primary--menu type--philosopher type--white type--heading"
          >Contact Us</nuxt-link>
        </div>
      </div>
    </nav>
    <Nuxt />
  </div>
</template>

<style>
</style>
