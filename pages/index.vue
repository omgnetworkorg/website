<template>
  <div>
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <img src="@/assets/images/logo.png">
          <h2 class="subtitle">
            Decentralized and open source finance solution
          </h2>
        </div>
      </div>
    </section>

    <section
      class="section link"
      @click="$router.push('/learn')">
      <div class="container">
        <h2 class="theme">LEARN</h2>
        <div class="subtitle">
          Educate yourself on the OMG Network components. 🎓
        </div>
        <nuxt-link
          to="/learn"
          class="learn-more">
          Learn more →
        </nuxt-link>
      </div>
    </section>

    <section
      class="section link has-text-right"
      @click="$router.push('/build')">
      <div class="container">
        <h2 class="theme">BUILD</h2>
        <div class="subtitle">
          🔧 Developers, explore the (open) source code and start tinkering.
        </div>
        <nuxt-link
          to="/build"
          class="learn-more">
          Learn more →
        </nuxt-link>
      </div>
    </section>
    <section
      class="section link"
      @click="$router.push('/contribute')">
      <div class="container">
        <h2 class="theme">CONTRIBUTE</h2>
        <div class="subtitle">
          Join our community to make the OMG Network thrive. 🤘
        </div>
        <nuxt-link
          to="/contribute"
          class="learn-more">
          Learn more →
        </nuxt-link>
      </div>
    </section>

    <Mission/>
  </div>
</template>

<script>
import Mission from '@/components/Mission'

export default {
  layout: 'empty',
  components: {
    Mission
  }
}
</script>

<style lang="scss" scoped>
section.hero {
  text-align: center;
  background: #1a53f0;
  img {
    width: 100px;
  }
  .hero-body {
    padding-top: 2rem;
    padding-bottom: 2rem;
  }
  .subtitle {
    color: rgba(255, 255, 255, .6);
    font-size: 1.5rem;
    padding-top: .5rem;
    font-family: 'Circular Std Book Italic', sans-serif;
  }
}
section.link {
  font-family: 'Open sans', sans-serif;
  padding-top: 3rem;
  padding-bottom: 3rem;
  padding-left: 2rem;
  padding-right: 2rem;
  border-bottom: 1px solid #eee;
  cursor: pointer;
  &:hover .learn-more {
    text-decoration: underline;
  }
  .learn-more {
    font-size: .75rem;
    color: inherit;
  }
  h2.theme {
    font-size: 2.2rem;
    margin-bottom: .25rem;
  }
  .subtitle {
    margin-bottom: .75rem;
    font-size: 1.5rem;
    font-family: 'Open Sans', sans-serif;
  }
}
</style>
