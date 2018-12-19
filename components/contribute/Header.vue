<template>
  <section class="section no-padding-v">
    <div class="container">
      <div class="subtitle">Whether you are a developer, a blockchain or decentralized finance enthusiast or just like helping out, you are welcome to help make OMG even better.</div>

      <div class="tabs">
        <ul>
          <li :class="{'is-active': $route.path === '/contribute'}">
            <nuxt-link to="/contribute">GROUPS</nuxt-link>
          </li>
          <li :class="{'is-active': $route.path === '/contribute/updates'}">
            <nuxt-link to="/contribute/updates">UPDATES</nuxt-link>
          </li>
          <li :class="{'is-active': $route.path === '/contribute/contributors'}">
            <nuxt-link to="/contribute/contributors">CONTRIBUTORS</nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.subtitle {
  padding-top: 2rem;
  font-family: 'Circular Std Book';
  font-size: 1.5rem;
  @media screen and (max-width: 640px) {
    font-size: 1.25rem;
  }
}
div.tabs {
  margin-bottom: 2rem;
  @media screen and (max-width: 640px) {
    font-size: .75rem;
  }
}
</style>
