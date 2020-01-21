<template>
  <section id="sidebar">
    <div class="logo-container">
      <img src="../assets/logo.png" id="logo">
    </div>
    <b-menu>
      <b-menu-list>
        <b-menu-item
          :active="isActive"
          icon-pack="redonicos"
          icon="icon-home"
          label="Painel"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-file"
          label="Minhas Redações"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-propostas"
          label="Propostas"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-simulados-2"
          label="Simulados"
        />
      </b-menu-list>
      <b-menu-list label="Biblioteca">
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-videoaulas"
          label="Videoaulas"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-materiais"
          label="Materias"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-coletaneas"
          label="Coletâneas"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-redacao"
          label="Folhas de Redação"
        />
        <b-menu-item
          icon-pack="redonicos"
          icon="icon-tutoriais is-medium"
          label="Tutoriais"
        />
      </b-menu-list>
    </b-menu>
  </section>
</template>

<script>

export default {
  name: 'Sidebar',
  data() {
    return {
      'isActive': true,
    }
  },
}
</script>

<style>
.menu {
  font-size: 0.95rem;
}

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
  font-weight: bold;
  border-left: 5px solid #EC8700;
  padding-left: 7px;
}

.icon.is-small {
  margin-left: 7px;
  margin-right: 15px;
  margin-top: 3px !important;
}

.redonicos, span {
  display: inline-block;
  vertical-align: middle;
}
</style>

<style scoped>
.logo-container {
  background: transparent linear-gradient(114deg, #EBAE1D 0%, #EA5703 51%, #D9000F 100%) 0% 0% no-repeat padding-box;
  opacity: 1;
  display: flex;
  justify-content: center;
}

#logo {
  margin-top: 6px;
  margin-bottom: 13px;
  width: 57%;
  height: 57%;
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
