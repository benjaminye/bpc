<template>
  <div>
    <nav class="nav">
      <header class="header">
        <a href="#" class="header__link">
          <img
            src="~/assets/img/logo-light.svg"
            alt="Bellwood Partners Logo"
            class="header__logo-img"
          />
          <h1 class="header__logo-text logo-text">
            Bellwood
            <br />Partners & Co
          </h1>
        </a>
      </header>
      <div class="menu">
        <div class="menu__column">
          <a href="#" class="menu__column-item menu-text">Services</a>
          <hr class="menu__column-divider" />
          <a href="#" class="menu__column-item menu-text">Case Studies</a>
        </div>
        <div class="menu__column">
          <a href="#" class="menu__column-item menu-text">Insights</a>
          <hr class="menu__column-divider" />
          <a href="#" class="menu__column-item menu-text">About</a>
        </div>
        <div class="menu__column">
          <a href="#" class="btn-primary btn-primary--menu menu-text">Contact Us</a>
        </div>
      </div>
    </nav>
    <Nuxt />
  </div>
</template>

<style>
</style>
