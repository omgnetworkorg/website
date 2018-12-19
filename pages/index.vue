<template>
  <div>
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            OMGNETWORK.ORG
          </h1>
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
        <h2 class="lbl">LEARN</h2>
        <h2 class="subtitle">
          Educate yourself on the OMG Network components. 🎓
        </h2>
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
        <h2 class="lbl">BUILD</h2>
        <h2 class="subtitle">
          🔧 Developers, explore the (open) source code and start tinkering.
        </h2>
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
        <h2 class="lbl">CONTRIBUTE</h2>
        <h2 class="subtitle">
          Join our community to make the OMG Network thrive. 🤘
        </h2>
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
}
section.link {
  font-family: 'Open sans', sans-serif;
  padding-top: 4rem;
  padding-bottom: 4rem;
  border-bottom: 1px solid #eee;
  cursor: pointer;
  &:hover .learn-more {
    text-decoration: underline;
  }
  .learn-more {
    font-size: .75rem;
    color: inherit;
  }
}
h2.lbl {
  margin-bottom: .75rem;
}
h2.subtitle {
  margin-bottom: .75rem;
  font-size: 1.5rem;
}
</style>
