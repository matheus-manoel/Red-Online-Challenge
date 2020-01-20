<template>
  <section id="sidebar">
    <div class="logo-container">
      <img src="../assets/logo.png" id="logo">
    </div>
    <b-menu>
      <b-menu-list>
        <span class="icon-home" />
        <b-icon pack="redonicons" icon="icon-home"></b-icon>
        <b-menu-item icon-pack="redonicons" icon="icon-home" label="Info"></b-menu-item>
      </b-menu-list>
      <b-menu-list label="Biblioteca">
        <b-menu-item icon="information-outline" label="Info"></b-menu-item>
      </b-menu-list>
    </b-menu>
  </section>
</template>

<script>
const customIconConfig = {
  customIconPacks: {
    'redonicons': {
      sizes: {
        'default': 'is-size-5',
        'is-small': '',
        'is-medium': 'is-size-3',
        'is-large': 'is-size-1'
      },
      internalIcons: {
        'icon-home': 'icon-home',
      }
    }
  }
}

export default {
  name: 'Sidebar',
  created() {
    this.$buefy.config.setOptions(customIconConfig)
  }
}
</script>

<style scoped>
@import "https://file.myfontastic.com/SBqPSxgJ9ZpScWYRpfw4ga/icons.css";
</style>

<style>
.logo-container {
  background: transparent linear-gradient(114deg, #D9000F 0%, #EA5703 51%, #EBAE1D 100%) 0% 0% no-repeat padding-box;
  opacity: 1;
  display: flex;
  justify-content: center;
}

#logo {
  margin-top: 6px;
  margin-bottom: 13px;
}

#sidebar {
  background-color: #FFFFFF;
  min-height: 100vh;
}
</style>
