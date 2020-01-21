<template>
  <section id="sidebar">
    <div class="logo-container">
      <img src="../assets/logo.png" id="logo">
    </div>
    <b-menu>
      <b-menu-list>
        <!--<b-icon pack="redonicons" icon="icon-home"></b-icon>-->
        <b-menu-item :active="isActive" icon="icon-home" label="Painel"></b-menu-item>
        <b-menu-item icon="a" label="Minhas Redações"></b-menu-item>
        <b-menu-item icon="a" label="Propostas"></b-menu-item>
        <b-menu-item icon="a" label="Simulados"></b-menu-item>
      </b-menu-list>
      <b-menu-list label="Biblioteca">
        <b-menu-item icon="information-outline" label="Videoaulas"></b-menu-item>
        <b-menu-item icon="information-outline" label="Materias"></b-menu-item>
        <b-menu-item icon="information-outline" label="Coletâneas"></b-menu-item>
        <b-menu-item icon="information-outline" label="Folhas de Redação"></b-menu-item>
        <b-menu-item icon="information-outline" label="Tutoriais"></b-menu-item>
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
  },
  data() {
    return {
      'isActive': true,
    }
  },
}
</script>

<style>
.menu-list a {
  border-radius: 0;
}

.menu-list a {
  color: #B3AFB3;
}

.menu-list a:hover {
  border-left: 5px solid #B3AFB3;
  color: #B3AFB3;
  padding-left: 7px;
}

.menu-list a.is-active {
  background: #F5B40026 0% 0% no-repeat padding-box;
  opacity: 1;
  color: #A5220C;
  border-left: 5px solid #EC8700;
  padding-left: 7px;
}
</style>

<style scoped>
@import "https://file.myfontastic.com/SBqPSxgJ9ZpScWYRpfw4ga/icons.css";

.logo-container {
  background: transparent linear-gradient(114deg, #EBAE1D 0%, #EA5703 51%, #D9000F 100%) 0% 0% no-repeat padding-box;
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

.menu-label {
  padding-left: 10px;
  border-radius: 0;
}
</style>
