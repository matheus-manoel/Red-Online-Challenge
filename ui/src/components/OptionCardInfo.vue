<template>
  <div class="section-info">
    <p class="subtitle">{{ title }}</p>
    <a href="/">{{ actionName }}</a>
  </div>
</template>

<script>
export default {
  name: 'OptionCardInfo',
  props: ['title', 'actionName'],
}
</script>

<style scoped>
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
</style>
