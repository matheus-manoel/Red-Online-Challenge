<template>
  <div>
    <div class="container" id="welcome-container">
      <p id="hello-msg">Olá, bem-vindo de volta, Gerald!</p>
    </div>
    <div class="container" id="inner-content-container">
    <div class="tile is-ancestor">
      <div class="tile is-parent is-7">
        <article class="tile is-child card" id="library-options-card">
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
          <LastProposals />
        </article>
      </div>
    </div>
    <div class="tile is-ancestor">
      <div class="tile is-parent">
        <article class="tile is-child card">
          <OptionCard
            title="Subir Nova Redação"
            actionName="Faça O Upload"
          />
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child card">
          <OptionCard
            title="Minhas Redações"
            actionName="Acessar"
          />
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child card">
          <OptionCard
            title="Visualizar Simulados"
            actionName="Acessar"
          />
        </article>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
import LibraryOption from './LibraryOption'
import LastProposals from './LastProposals'
import OptionCard from './OptionCard'

export default {
  name: 'StudentPanel',
  components: {
    LibraryOption,
    LastProposals,
    OptionCard,
  },
}
</script>

<style>
#welcome-container {
  background-color: #FDEFD7;
}

#welcome-container p {
  padding: 5px 10px 5px 40px;
}

#inner-content-container {
  margin: 40px;
  background-color: #FFFBEF;
}

#hello-msg {
  color: #A5220C;
  font-family: proximaNovaSemiBold;
}

#library-options-card {
  padding: 45px 66px;
}

.library-options {
  display: flex;
  flex-direction: row;
}
</style>
