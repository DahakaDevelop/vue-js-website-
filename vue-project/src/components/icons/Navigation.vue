<template>
  <nav class="navigation">
    <div class="logo">
      <img :src="logo" alt="Logo" />
    </div>
    <ul class="navigation__list">
      <li class="navigation__item" v-for="(link, index) in links" :key="index">
        <a :href="link.url" :class="{ 'active': activeLink === link.label }">{{ link.label }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    logo: {
      type: String,
      required: true
    },
    links: {
      type: Array,
      required: true
    },
    activeLink: {
      type: String,
      required: true
    }
  }
}
</script>

<style>
/* add styles for the navigation component */
</style>