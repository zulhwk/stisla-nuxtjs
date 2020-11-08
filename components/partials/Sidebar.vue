<template>
  <div class="main-sidebar">
    <aside id="sidebar-wrapper">
      <div class="sidebar-brand">
        <nuxt-link to="#">
          Stisla NuxtJS
        </nuxt-link>
      </div>
      <div class="sidebar-brand sidebar-brand-sm">
        <nuxt-link to="#">
          St
        </nuxt-link>
      </div>
      <!-- MAIN CONTENT SIDEBAR -->
      <ul class="sidebar-menu">
        <li class="menu-header">
          Dashboard
        </li>
        <li class="nav-item dropdown active">
          <a style="cursor:pointer;" class="nav-link has-dropdown" @click="toggleMenu">
            <i class="fas fa-fire" /> <span>Dashboard</span>
          </a>
          <ul :class="'dropdown-menu ' + showMenus">
            <li>
              <nuxt-link class="nav-link" to="index-0.html">
                General Dashboard
              </nuxt-link>
            </li>
            <li class="active">
              <nuxt-link class="nav-link" to="index-0.html">
                Ecommerce Dashboard
              </nuxt-link>
            </li>
          </ul>
        </li>
        <li>
          <a class="nav-link" href="blank.html">
            <i class="fas fa-home" /> <span>Blank Page</span>
          </a>
        </li>
      </ul>
    </aside>
  </div>
</template>

<script>
export default {
  data () {
    return {
      activeMenu: false,
      showMenus: ''
    }
  },
  methods: {
    toggleMenu () {
      if (this.activeMenu === false) {
        //
        this.activeMenu = !this.activeMenu
        this.showMenus = 'menuActive'
      } else {
        //
        this.activeMenu = !this.activeMenu
        this.showMenus = ''
      }
    }
  }
}
</script>
