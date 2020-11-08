<template>
  <div class="body_blog">
    <Navbar :class="navFixed" />
    <Nuxt />
  </div>
</template>

<script>
import Navbar from '@/layouts/partials/blog/Navbar.vue'
export default {
  components: {
    Navbar
  },
  data () {
    return {
      navFixed: ''
    }
  },
  mounted () {
    window.addEventListener('scroll', this.navbarFixed)
  },
  methods: {
    navbarFixed () {
      if (window.scrollY >= 150) {
        this.navFixed = 'fixed-nav'
      } else {
        this.navFixed = ''
      }
    }
  },
  head: {
    link: [
      { rel: 'stylesheet', src: require('@/assets/css/style.css') }
    ]
  }
}
</script>
