<template>
  <div class="columns">
    <div class="column is-2" id="sidebar-container">
      <Sidebar />
    </div>
    <div class="column" id="content-container">
      <Navbar />
      <StudentPanel />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue'
import StudentPanel from './components/StudentPanel.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'app',
  components: {
    Sidebar,
    StudentPanel,
    Navbar,
  }
}
</script>

<style>
html {
  background-color: #FFFBEF;
  min-height: 100vh;
}

body {
  min-height: 100vh;
}

.columns {
  margin-bottom: 0;
}

.column {
  min-height: 100vh;
}

#sidebar-container {
  padding-right: 0;
  background-color: #FFFFFF;
  padding-bottom: 0;
}

#content-container {
  padding-left: 0;
  padding-right: 0;
}
</style>

