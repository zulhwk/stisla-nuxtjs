<template>
  <div class="main-wrapper">
    <div class="navbar-bg" />
    <Navbar />
    <Sidebar />
  </div>
</template>

<script>
import Navbar from '@/layouts/partials/NavbarLeft.vue'
import Sidebar from '@/layouts/partials/Sidebar.vue'
export default {
  layout: 'admin',
  components: {
    Navbar,
    Sidebar
  }
}
</script>
