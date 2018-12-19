<template>
  <div>
    <ContributeHeader/>

    <section class="section contributors no-padding-v">
      <div class="container">
        <div class="columns is-mobile is-multiline">
          <div
            v-for="(contributor, username) in contributors"
            :key="username"
            class="column is-one-fifth-desktop is-half-mobile">
            <img :src="contributor.avatar">
            <strong>{{ contributor.name }}</strong>
            <span class="oneliner">{{ contributor.oneliner }}</span>
          </div>
        </div>
      </div>
    </section>

  </div>
</template>

<script>
import ContributeHeader from '@/components/contribute/Header'
import contributors from '@/assets/contributors'

export default {
  components: {
    ContributeHeader
  },
  data () {
    return {
      contributors
    }
  }
}
</script>

<style lang="scss" scoped>
.contributors {
  font-size: .9rem;
  img {
    width: 100%;
  }
  span.oneliner {
    display: block;
  }
}
</style>
