<template>
  <div>
    <div class="container" id="welcome-container">
      <p>Olá, bem-vindo de volta, Gerald!</p>
      <span class="icon-home">test</span>
    </div>
    <div class="container" id="inner-content-container">
    <div class="tile is-ancestor">
      <div class="tile is-parent is-7">
        <article class="tile is-child card">
          <p class="title">Hello World</p>
          <p class="subtitle">What is up?</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child card">
          <p class="title">Foo</p>
          <p class="subtitle">Bar</p>
        </article>
      </div>
    </div>
    <div class="tile is-ancestor">
      <div class="tile is-parent">
        <article class="tile is-child card">
          <p class="title">Hello World</p>
          <p class="subtitle">What is up?</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child card">
          <p class="title">Foo</p>
          <p class="subtitle">Bar</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child card">
          <p class="title">Foo</p>
          <p class="subtitle">Bar</p>
        </article>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StudentPanel',
}
</script>

<style>
#welcome-container {
  background-color: #FDEFD7;
}

#welcome-container p {
  padding: 10px;
  padding-left: 40px;
}

#inner-content-container {
  margin: 50px;
  background-color: #FFFBEF;
}
</style>
