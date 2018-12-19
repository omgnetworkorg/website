<template>
  <section class="section">
    <div class="container">
      <div class="subtitle">Developers, building applications for the OMG Network is already possible, even though the network is not running yet. Find resources below.</div>

      <h2 class="title">OmiseGO eWallet</h2>
      <ul>
        <li>
          <a
            href="https://github.com/omisego/ewallet"
            target="_blank">Github</a>
          Open source code of the eWallet SDK
        </li>
        <li>
          <a
            href="https://github.com/omisego/ewallet/blob/master/docs/demo.md"
            target="_blank">Demo</a>
          Explore the sample shop server demos without setting up your own.
        </li>
        <li>
          <a
            href="https://github.com/omisego/ewallet/blob/master/docs/guides/guides.md"
            target="_blank">Guides</a>
          Understand how the eWallet server works behind the scene.
        </li>
        <li>
          <a
            href="https://github.com/omisego/ewallet/blob/master/docs/design/design.md"
            target="_blank">Design</a>
          Find out about the technical design decisions that revolve around the eWallet server.
        </li>
        <li>
          <a
            href="https://github.com/omisego/ewallet/blob/master/docs/tests/tests.md"
            target="_blank">Tests</a>
          See how tests are organized for the eWallet server.
        </li>
        <li>
          <a
            href="https://github.com/omisego/ewallet/blob/master/docs/faq.md"
            target="_blank">FAQ</a>
          Frequently asked questions.
        </li>
      </ul>

      <h2 class="title">eWallet client libraries</h2>
      <ul>
        <li>
          <a
            href="https://github.com/Alainy/OmiseGo-Go-SDK"
            target="_blank">GoLang</a>
          by @Alainy
        </li>
      </ul>

      <h2 class="title">Plasma</h2>
      <ul>
        <li>
          <a
            href="https://github.com/omisego/plasma-contracts"
            target="_blank">OmiseGO Plasma Contracts</a>
          open source code on Github
        </li>
        <li>
          <a
            href="https://github.com/omisego/elixir-omg"
            target="_blank">elixir-omg</a>
          OmiseGO's Elixir implementation of Plasma and basis for the OMG Network
        </li>
      </ul>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.subtitle {
  font-family: 'Circular Std Book';
  padding-bottom: 2rem;
  font-size: 1.5rem;
  @media screen and (max-width: 640px) {
    font-size: 1.25rem;
  }
}
@media screen and (max-width: 640px) {
  h2.title {
    font-size: 1.5rem;
  }
}
ul {
  margin-bottom: 3rem;
}
</style>
