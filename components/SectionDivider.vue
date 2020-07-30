<template>
  <div class="section-divider">
    <hr class="section-divider__line" />
    <h2 class="section-divider__text type--raleway type--subheading type--secondary">
      <slot></slot>
    </h2>
    <hr class="section-divider__line" />
  </div>
</template>

<script>
export default {
  props: ["dividerText"],
};
</script>

<style>
</style>