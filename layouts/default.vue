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
            <img
              src="https://bulma.io/images/bulma-logo.png"
              width="112"
              height="28">
          </nuxt-link>

          <a
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarHeader">
            <span aria-hidden="true"/>
            <span aria-hidden="true"/>
            <span aria-hidden="true"/>
          </a>
        </div>

        <div
          id="navbarHeader"
          class="navbar-menu">

          <div class="navbar-end">

            <!--
            <nuxt-link
              :to="item.to"
              exact-active-class="is-active">
              <b-icon :icon="item.icon"/> {{ item.title }}
            </nuxt-link>
             -->
            <nuxt-link
              to="/learn"
              class="navbar-item">
              LEARN
            </nuxt-link>
            <nuxt-link
              to="/build"
              class="navbar-item">
              BUILD
            </nuxt-link>
            <nuxt-link
              to="/contribute"
              class="navbar-item">
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
  background: #2B2B2B;
}
.navbar-end .navbar-item {
  font-family: 'Raleway', sans-serif;
  font-size: .8rem;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
  &.nuxt-link-active {
    border-bottom: 3px solid #fff;
    padding-top: 11px;
  }
}
</style>
