<template>
  <main class="app-home">
    <appHeader class="full" />
    <appHero />
    <cardList />
    <appSection />
    <testimonialList />
    <formCta />
    <appFooter />
  </main>
</template>

<script>
import appHeader from './cmps/app-header.vue'
import appHero from './cmps/app-hero.vue'
import cardList from './cmps/card-list.vue'
import appSection from './cmps/app-section.vue'
import testimonialList from './cmps/testimonial-list.vue'
import formCta from './cmps/form-cta.vue'
import appFooter from './cmps/app-footer.vue'

export default {
  components: {
    appHeader,
    appHero,
    cardList,
    appSection,
    testimonialList,
    formCta,
    appFooter,
  },
}
</script>

<style scoped></style>
