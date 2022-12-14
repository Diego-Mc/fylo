<template>
  <article class="testimonial-preview">
    <p class="text">{{ text }}</p>
    <footer class="footer">
      <img
        class="person-img"
        :src="'../src/assets/imgs/' + personImgName"
        alt="person-img" />
      <h6 class="person-name">{{ personName }}</h6>
      <small class="person-desc">{{ personDesc }}</small>
    </footer>
  </article>
</template>

<script>
export default {
  props: {
    text: String,
    personImgName: String,
    personName: String,
    personDesc: String,
  },
}
</script>

<style lang="scss" scoped></style>
