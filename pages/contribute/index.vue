<template>
  <div>
    <ContributeHeader/>

    <section class="section groups no-padding-v">
      <div class="container">

        <div class="subtitle">We have entry points for various themes, and anyone is free to join a group at any time :</div>

        <div class="group">
          <h3 class="lbl">Core</h3>
          <p>The core team is mostly OmiseGO, but welcomes outside help. You are or want to become a blockchain developer, you'll be able to contribute to the most technical pieces of the OMG network architecture by writing code, triaging issues, reviewing pull requests and debating development decisions.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>
        <div class="group">
          <h3 class="lbl">Education</h3>
          <p>The education team makes sure the OMG network is accessible by updating the OMG Network Guide, writing technical documentation and preparing focused documents on trending subjects.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>
        <div class="group">
          <h3 class="lbl">Support</h3>
          <p> In parallel to the education mission, answering the community's questions and concerns is a never ending task that has a tremendous importance to welcome fellow OMGers. If you have even a very shallow OMG knowledge, it is a great way to start contributing to the community and even educate yourself on the way.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>
        <div class="group">
          <h3 class="lbl">Community</h3>
          <p>If meetups and conferences are more your thing, the Community Slack channel is the best place to start. This group intends to support all sort of events to expand our community to new horizons.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>
        <div class="group">
          <h3 class="lbl">Tokenomy</h3>
          <p>The tokenomy group focuses on making sure the network is healthy by securing the value of the tokens and monitoring its activity. They are also in charge of the different staking challenges.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>
        <div class="group">
          <h3 class="lbl">Tooling</h3>
          <p>Creating the necessary tooling for our community to thrive brings its own set of challenges. Seasoned open source contributors can provide very valuable input here.</p>
          <a
            href=""
            class="learn-more">
            Learn more →
          </a>
        </div>

      </div>
    </section>

  </div>
</template>

<script>
import ContributeHeader from '@/components/contribute/Header'

export default {
  components: {
    ContributeHeader
  }
}
</script>

<style lang="scss" scoped>
.groups {
  .subtitle {
    margin-bottom: .5rem;
    font-family: 'Circular Std Book Italic';
  }
}
.group {
  padding: 2rem 0;
  border-bottom: 1px solid #eee;
  cursor: pointer;
  h3.lbl {
    font-weight: bold;
    text-transform: uppercase;
    margin-bottom: .75rem;
    font-size: .9rem;
  }
  .learn-more {
    font-size: .75rem;
    color: inherit;
    margin-top: 1rem;
  }
  &:hover .learn-more {
    text-decoration: underline;
  }
}
</style>

