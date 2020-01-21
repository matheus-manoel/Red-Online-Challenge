<template>
  <div>
    <div class="container" id="welcome-container">
      <p id="hello-msg">Olá, bem-vindo de volta, Gerald!</p>
    </div>
    <div class="container" id="inner-content-container">
    <div class="tile is-ancestor">
      <div class="tile is-parent is-7">
        <article class="tile is-child card">
          <p class="subtitle">Acesse A Biblioteca:</p>
          <div class="library-options">
            <LibraryOption />
            <LibraryOption />
            <LibraryOption />
            <LibraryOption />
            <LibraryOption />
          </div>
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
import LibraryOption from './LibraryOption'

export default {
  name: 'StudentPanel',
  components: {
    LibraryOption,
  },
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

#hello-msg {
  color: #A5220C;
  font-weight: bold;
}

.card {
  padding: 45px 66px;
}

.library-options {
  display: flex;
  flex-direction: row;
}
</style>
