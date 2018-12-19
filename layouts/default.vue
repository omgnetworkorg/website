<template>
  <div>

    <nav
      class="navbar is-fixed-top is-dark"
      role="navigation"
      aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <nuxt-link
            class="navbar-item"
            to="/">
            <img src="@/assets/images/logo.png">
          </nuxt-link>

          <a
            :aria-expanded="expandMenu"
            :class="{ 'is-active': expandMenu }"
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            @click="expandMenu = !expandMenu">
            <span aria-hidden="true"/>
            <span aria-hidden="true"/>
            <span aria-hidden="true"/>
          </a>
        </div>

        <div
          id="navbarHeader"
          :class="{ 'is-active': expandMenu }"
          class="navbar-menu">
          <div class="navbar-start"/>
          <div class="navbar-end">
            <nuxt-link
              to="/learn"
              class="navbar-item"
              @click.native="expandMenu = false">
              LEARN
            </nuxt-link>
            <nuxt-link
              to="/build"
              class="navbar-item"
              @click.native="expandMenu = false">
              BUILD
            </nuxt-link>
            <nuxt-link
              to="/contribute"
              class="navbar-item"
              @click.native="expandMenu = false">
              CONTRIBUTE
            </nuxt-link>
          </div>
        </div>
      </div>
    </nav>

    <nuxt />

  </div>
</template>

<script>
export default {
  head: {
    bodyAttrs: {
      class: 'has-navbar-fixed-top'
    }
  },
  data() {
    return {
      expandMenu: false,
      items: [
        { title: 'Home', icon: 'home', to: { name: 'index' } },
        { title: 'Inspire', icon: 'lightbulb', to: { name: 'inspire' } }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.navbar {
  background: #1a53f0;
}
.navbar.is-dark .navbar-brand .navbar-item:hover {
  background: transparent;
}
.navbar.is-dark a.navbar-item:hover {
  background-color: transparent;
}
.navbar-end .navbar-item {
  font-family: 'Std Circular Black', sans-serif;
  font-size: .85rem;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
  &.nuxt-link-active {
    border-bottom: 3px solid #fff;
    padding-top: 11px;
  }
}
</style>
