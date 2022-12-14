<template>
  <article class="card-preview">
    <img class="img" :src="'../src/assets/imgs/' + imgName" alt="card-img" />
    <h3 class="title">{{ title }}</h3>
    <p class="desc">{{ desc }}</p>
  </article>
</template>

<script>
export default {
  props: {
    title: String,
    desc: String,
    imgName: String,
  },
}
</script>

<style lang="scss" scoped></style>
