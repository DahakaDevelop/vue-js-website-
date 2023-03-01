<template>
  <section class="hero" :style="{ backgroundImage: `url(${backgroundImage})` }">
    <div class="hero__content">
      <h1 class="hero__title">{{ title }}</h1>
      <p class="hero__subtitle">{{ subtitle }}</p>
      <a class="hero__button" :href="ctaButton.url">{{ ctaButton.label }}</a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    title: {
      type: String,
      required: true
    },
    subtitle: {
      type: String,
      required: true
    },
    backgroundImage: {
      type: String,
      required: true
    },
    ctaButton: {
      type: Object,
      required: true
    }
  }
}
</script>

<style>
/* add styles for the hero component */
</style>