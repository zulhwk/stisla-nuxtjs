<template>
  <div class="main-wrapper">
    <div class="navbar-bg" />
    <Navbar />
    <Sidebar />
  </div>
</template>

<script>
import Navbar from '@/components/partials/NavbarLeft.vue'
import Sidebar from '@/components/partials/Sidebar.vue'
export default {
  layout: 'admin',
  components: {
    Navbar,
    Sidebar
  }
}
</script>
