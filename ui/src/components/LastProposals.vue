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
    <OptionCardInfo title="Últimas Propostas" actionName="Acessar"/>
  </section>
</template>

<script>
import OptionCardInfo from './OptionCardInfo'

export default {
  name: 'LastProposals',
  components: {
    OptionCardInfo,
  }
}
</script>

<style scoped>
.columns {
  margin: 0;
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
