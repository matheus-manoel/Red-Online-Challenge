<template>
    <section>
    <div class="container wrapper">
      <div class="columns">
        <div class="column is-6 has-text-centered icon-wrapper">
          <span class="icon-surface" />
        </div>
        <div class="column">
        </div>
      </div>
    </div>
    <OptionCardInfo />
    </section>
</template>

<script>
import OptionCardInfo from './OptionCardInfo'

export default {
  'name': 'OptionCard',
  'components': {
    OptionCardInfo,
  }
}
</script>

<style scoped>
.columns {
  background: transparent linear-gradient(294deg, #D9000F 0%, #EA5703 55%, #EBAE1D 100%) 0% 0% no-repeat padding-box;
  margin: 0;
}

.icon-wrapper {
  color: #FFFFFF;
  font-size: 7rem;
  margin-top: -19px;
}

span {
  margin-bottom: -50px;
}
</style>
