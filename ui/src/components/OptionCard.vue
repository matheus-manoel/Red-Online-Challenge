<template>
    <section>
    <div class="container wrapper">
      <div
        class="columns" 
        :class="{
          'orange-gradient': isOrange,
          'pink-gradient': isPink,
          'yellow-gradient': isYellow
        }"
      >
        <div class="column is-6 has-text-centered icon-wrapper">
          <span :class="icon" />
        </div>
        <div class="column">
        </div>
      </div>
    </div>
    <OptionCardInfo
      v-bind:title="title"
      v-bind:actionName="actionName"
    />
    </section>
</template>

<script>
import OptionCardInfo from './OptionCardInfo'

export default {
  name: 'OptionCard',
  components: {
    OptionCardInfo,
  },
  props: ['title', 'actionName', 'icon', 'isOrange', 'isPink', 'isYellow'],
}
</script>

<style scoped>
.columns {
  margin: 0;
}

.orange-gradient {
  background: transparent linear-gradient(294deg, #D9000F 0%, #EA5703 55%, #EBAE1D 100%) 0% 0% no-repeat padding-box;
}

.pink-gradient {
  background: transparent linear-gradient(294deg, #F5317F 0%, #FF7C6E 100%) 0% 0% no-repeat padding-box;
}

.yellow-gradient {
  background: transparent linear-gradient(294deg, #FF8359 0%, #FFDF40 100%) 0% 0% no-repeat padding-box;
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
