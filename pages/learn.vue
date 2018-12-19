<template>
  <div class="container">
    <section class="section has-text-centered	get-started">
      <div class="subtitle">
        <strong>Get started</strong> with a non-technical introduction : the OMG Network Guide.
      </div>
      <a
        href="/guide"
        class="button is-large is-info"
        target="_blank">
        📘 Read the Guide
      </a>
      <a
        href="/guide/contribute.html"
        class="button is-large"
        target="_blank">
        👉 Contribute
      </a>
    </section>

    <section class="section resources">
      <h1 class="title">External resources</h1>
      <ul>
        <li>
          <a
            href="https://www.learnplasma.org/"
            target="_blank">LearnPlasma.org</a>
          The go-to resource to learn Plasma constructions
        </li>
      </ul>
    </section>

  </div>
</template>

<style lang="scss" scoped>
.get-started {
  padding-top: 5rem;
  padding-bottom: 3rem;
  .subtitle {
    margin-bottom: 3rem;
  }
  .button {
    margin-left: .5rem;
    margin-right: .5rem;
  }
  .button.is-info {
    margin-bottom: 1.5rem;
  }
}
.resources {
  .title {
    font-size: 2rem;
  }
  li a {
    font-weight: bold;
    color: inherit;
    text-decoration: underline;
  }
}
</style>
