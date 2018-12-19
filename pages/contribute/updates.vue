<template>
  <div>
    <ContributeHeader/>

    <section class="section no-padding-v">
      <div class="container">

        <article>
          <div class="article-header">
            <span class="group lbl">Tooling</span>
            <span class="date">December 14th, 2018</span>
          </div>
          <div class="subtitle">Website is online</div>
          <p>
            The website is finally online at <strong>omgnetwork.org</strong>, it intends to present our work and help onboard new contributors by presenting our activity.
          </p>
          <p>
            These posts should be quick updates, posted by the different work groups, to inform the rest of the community about their progress and/or current goals. They will be probably be hosted on Wordpress, or maybe a content publishing API.
          </p>
        </article>

        <article>
          <div class="article-header">
            <span class="group lbl">Education</span>
            <span class="date">December 9th, 2018</span>
          </div>
          <div class="subtitle">OMG Network Guide</div>
          <p>
            We have finalized a first version of the Guide, that is can be communicated to the public : <a
              href="https://omgnetwork.org/guide"
              target="_blank">https://omgnetwork.org/guide</a>
          </p>
          <p>
            It is hosted on Github, and powered by VuePress. Evolutions and comments will be handled via <a
              href="https://github.com/OMGnetwork/guide/issues"
              target="_blank">Github issues</a> and we opened a <a
                href="https://gitter.im/OMGnetwork/guide"
                target="_blank">Gitter channel</a>.
          </p>
        </article>

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
article {
  padding: 2rem 0;
  border-bottom: 1px solid #eee;
  &:first-child {
    padding-top: 0;
  }
  .article-header {
    .lbl {
      text-transform: uppercase;
      font-size: .75rem;
      margin-right: .5rem;
    }
    .date {
      font-size: .75rem;
      opacity: .8;
    }
  }
  .subtitle {
    margin: 1rem 0;
    font-size: 1.5rem;
    font-family: 'Circular Std Medium';
  }
  p {
    padding-bottom: .5rem;
    &:last-child {
      padding-bottom: 0;
    }
  }
}
</style>
