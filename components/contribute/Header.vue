<template>
  <div class="container">
    <h2 class="subtitle">Whether you are a developer, a blockchain or decentralized finance enthusiast or just like helping out, you are welcome to help make OMG even better.</h2>

    <div class="tabs">
      <ul>
        <li :class="{'is-active': $route.path === '/contribute'}">
          <nuxt-link to="/contribute">GROUPS</nuxt-link>
        </li>
        <li :class="{'is-active': $route.path === '/contribute/reports'}">
          <nuxt-link to="/contribute/reports">COMMUNITY REPORTS</nuxt-link>
        </li>
        <li :class="{'is-active': $route.path === '/contribute/contributors'}">
          <nuxt-link to="/contribute/contributors">CONTRIBUTORS</nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.subtitle {
  padding-top: 2rem;
}
</style>
