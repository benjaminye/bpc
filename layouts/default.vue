<template>
  <div>
    <input type="checkbox" class="burger-menu__checkbox" id="burger-menu" />
    <label class="burger-menu__label" for="burger-menu">
      <div class="burger-menu__icon">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </label>
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
        <div class="burger-menu">
          <span class="burger-menu__bar--1"></span>
          <span class="burger-menu__bar--2"></span>
          <span class="burger-menu__bar--3"></span>
        </div>
      </header>
      <div class="menu">
        <div class="menu__column">
          <nuxt-link
            to="/services/strategic-advisory"
            class="menu__column-item type--philosopher type--white type--heading"
            >Services</nuxt-link
          >
          <hr class="menu__column-divider" />
          <nuxt-link
            to="/cases"
            class="menu__column-item type--philosopher type--white type--heading"
            >Case Studies</nuxt-link
          >
        </div>
        <div class="menu__column">
          <nuxt-link
            to="/insights"
            class="menu__column-item type--philosopher type--white type--heading"
            >Insights</nuxt-link
          >
          <hr class="menu__column-divider" />
          <nuxt-link
            to="/about/mission"
            class="menu__column-item type--philosopher type--white type--heading"
            >About</nuxt-link
          >
        </div>
        <div class="menu__column">
          <nuxt-link
            to="/contact"
            class="menu__button btn-primary btn-primary--menu type--philosopher type--white type--heading"
            >Contact Us</nuxt-link
          >
        </div>
      </div>
    </nav>
    <Nuxt />
  </div>
</template>

<style></style>
