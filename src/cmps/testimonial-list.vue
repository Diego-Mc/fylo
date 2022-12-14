<template>
  <section class="testimonial-list">
    <testimonialPreview
      v-for="testimonial in testimonials"
      :text="testimonial.text"
      :personImgName="testimonial.personImgName"
      :personName="testimonial.personName"
      :personDesc="testimonial.personDesc" />
  </section>
</template>

<script>
import testimonialPreview from './testimonial-preview.vue'
export default {
  data() {
    return {
      testimonials: [
        {
          text: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
          personImgName: 'profile-1.jpg',
          personName: 'Satish Patel',
          personDesc: 'Founder & CEO, Huddle',
        },
        {
          text: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
          personImgName: 'profile-2.jpg',
          personName: 'Bruce McKenzie',
          personDesc: 'Founder & CEO, Huddle',
        },
        {
          text: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
          personImgName: 'profile-3.jpg',
          personName: 'Iva Boyd',
          personDesc: 'Founder & CEO, Huddle',
        },
      ],
    }
  },
  components: {
    testimonialPreview,
  },
}
</script>

<style lang="scss" scoped></style>
