<template>
  <div class>
    <div class="contact-content">
      <div class="contact-content__address">
        <h1
          class="contact-content__office type--raleway type--xlarge type--secondary type--underline"
        >Toronto Office</h1>
        <h2 class="contact-content__name type--raleway type--large type--primary">Justin Ulster</h2>
        <p
          class="contact-content__position contact-text type--libre-franklin type--subheading type--grey-dark-2"
        >Managing Partner</p>
        <a
          href="tel:+14162708568"
          class="contact-content__phone type--open-sans type--small type--secondary type--underline"
        >+1 (416) 270-8568</a>
        <a
          href="mailto:mail@mail.com"
          class="contact-content__email type--open-sans type--small type--secondary type--underline"
        >mail@mail.com</a>
      </div>
      <img src="~/assets/img/contact_splash.jpg" alt class="contact-splash" />
    </div>
    <footer-app></footer-app>
  </div>
</template>

<script>
import Footer from "@/components/Footer";

export default {
  name: "contact",
  head() {
    return {
      title: `BPC | Contact Us`,
    };
  },
  components: {
    "footer-app": Footer,
  },
};
</script>

<style></style>
