<template>
  <div class="container">
    <section class="section has-text-centered	get-started">
      <h2 class="subtitle">
        <strong>Get started</strong> with a non-technical introduction : the OMG Network Guide.
      </h2>
      <a
        href="/guide"
        class="button is-info"
        target="_blank">
        📘 Read the Guide
      </a>
      <a
        href="/guide/contribute.html"
        class="button"
        target="_blank">
        👉 Contribute
      </a>
    </section>

    <section class="section resources">
      <h1 class="title">Education resources</h1>
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
  .button.is-info {
    margin-right: 1rem;
  }
}
.resources {
  li a {
    font-weight: bold;
    color: inherit;
    text-decoration: underline;
  }
}
</style>
