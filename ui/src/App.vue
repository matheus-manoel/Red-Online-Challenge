<template>
  <div class="columns">
    <div class="column">
      <Sidebar />
    </div>
    <div class="column is-four-fifths">
      <StudentPanel />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue'
import StudentPanel from './components/StudentPanel.vue'

export default {
  name: 'app',
  components: {
    Sidebar,
    StudentPanel
  }
}
</script>

<style>
</style>
