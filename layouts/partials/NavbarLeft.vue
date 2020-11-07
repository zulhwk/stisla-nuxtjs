<template>
  <nav class="navbar navbar-expand-lg main-navbar">
    <b-form inline class="mr-auto">
      <ul class="navbar-nav mr-3">
        <li>
          <a style="cursor:pointer;" data-toggle="sidebar" class="nav-link nav-link-lg" @click="toggleSidebar">
            <i class="fas fa-bars" />
          </a>
        </li>
        <li>
          <a href="#" data-toggle="search" class="nav-link nav-link-lg d-sm-none">
            <i class="fas fa-search" />
          </a>
        </li>
      </ul>
      <Search />
    </b-form>
    <!-- PROFILE SECTION -->
    <ul class="navbar-nav navbar-right">
      <!-- EMAIL -->
      <li class="dropdown dropdown-list-toggle">
        <a href="#" data-toggle="dropdown" class="nav-link nav-link-lg message-toggle beep">
          <i class="far fa-envelope" />
        </a>
      </li>
      <!-- NOTIFIKASI -->
      <li class="dropdown dropdown-list-toggle">
        <a href="#" data-toggle="dropdown" class="nav-link notification-toggle nav-link-lg beep">
          <i class="far fa-bell" />
        </a>
      </li>
      <!-- PROFILE -->
      <li class="dropdown">
        <a href="#" data-toggle="dropdown" class="nav-link dropdown-toggle nav-link-lg nav-link-user">
          <img src="@/assets/stisla/img/avatar/avatar-1.png" alt="" class="rounded-circle mr-1">
          <div class="d-sm-none d-lg-inline-block">
            Hi, Ujang Maman
          </div>
        </a>
        <div class="dropdown-menu dropdown-menu-right">
          <a href="" class="dropdown-item has-icon">
            <i class="far fa-user" /> Profile
          </a>
          <a href="" class="dropdown-item has-icon">
            <i class="fas fa-cog" /> Setting
          </a>
          <a href="" class="dropdown-item has-icon">
            <i class="fas fa-cog" /> Logout
          </a>
        </div>
      </li>
    </ul>
  </nav>
</template>

<script>
import Search from '@/layouts/partials/Search.vue'
export default {
  components: {
    Search
  },
  methods: {
    toggleSidebar () {
      const win = document.body
      if (win.classList.value === 'sidebar-mini') {
        win.classList.remove('sidebar-mini')
      } else {
        win.classList.add('sidebar-mini')
      }
    }
  }
}
</script>
