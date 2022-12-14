<template>
  <section class="card-list">
    <cardPreview
      v-for="card in cards"
      :title="card.title"
      :imgName="card.imgName"
      :desc="card.desc" />
  </section>
</template>

<script>
import cardPreview from './card-preview.vue'
export default {
  data() {
    return {
      cards: [
        {
          imgName: 'card-1.svg',
          title: 'Access your files, anywhere',
          desc: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.',
        },
        {
          imgName: 'card-2.svg',
          title: 'Security you can trust',
          desc: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.',
        },
        {
          imgName: 'card-3.svg',
          title: 'Real-time collaboration',
          desc: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.',
        },
        {
          imgName: 'card-4.svg',
          title: 'Store any type of file',
          desc: "Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.",
        },
      ],
    }
  },
  components: {
    cardPreview,
  },
}
</script>

<style lang="scss" scoped></style>
