<template>
  <div>
    <Sidebar />
    <StudentPanel />
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
