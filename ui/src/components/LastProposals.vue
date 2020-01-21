<template>
  <section>
    <div class="section-container">
      <div v-for="i in 5" v-bind:key="i">
        <div class="columns">
          <div class="column is-narrow title-column" id="title-column">
            <p>Caminhos para a melhoria da segurança pública no Brasil</p>
          </div>
          <div class="column subitem-column has-text-right">
            <p>ENEM</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section-info">
      <p class="subtitle">Últimas Propostas</p>
      <a href="/">Acessar</a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'LastProposals',
}
</script>

<style scoped>
.columns {
  margin: 0;
}

a:hover {
  color: #EE9823;
}

.section-info {
  padding: 15px 30px;
}

.subtitle {
  margin-bottom: 0px;
  font-family: proximaNovaSemiBold;
}

.section-container {
  background: transparent linear-gradient(110deg, #7596F6 0%, #69ABF5 100%) 0% 0% no-repeat padding-box;
  color: #FFFFFF;
  padding: 10px 20px;
}

.title-column {
  padding: 3px 0;
}

.subitem-column {
  padding: 3px 0;
}
</style>
