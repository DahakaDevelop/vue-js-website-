<template>
  <div class="testimonial">
    <div class="testimonial__avatar">
      <img :src="avatar" alt="Testimonial Author Avatar" />
    </div>
    <div class="testimonial__content">
      <p class="testimonial__text">{{ content }}</p>
      <p class="testimonial__author">{{ author }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Testimonial',
  props: {
    avatar: {
      type: String,
      required: true
    },
    author: {
      type: String,
      required: true
    },
    content: {
      type: String,
      required: true
    }
  }
}
</script>

<style>
/*
