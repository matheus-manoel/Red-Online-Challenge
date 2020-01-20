<template>
  <section id="sidebar">
    <div class="logo-container">
      <img src="../assets/logo.png" id="logo">
    </div>
    <b-menu>
      <b-menu-list>
        <b-menu-item icon="information-outline" label="Info"></b-menu-item>
        <b-menu-item
          icon="settings"
          :active="isActive"
          :expanded="isActive"
          @click="isActive = !isActive">
          <template slot="label" slot-scope="props">
            Administrator
            <b-icon
              class="is-pulled-right"
              :icon="props.expanded ? 'menu-down' : 'menu-up'">
            </b-icon>
          </template>
          <b-menu-item icon="account" label="Users"></b-menu-item>
          <b-menu-item icon="cellphone-link">
            <template slot="label" slot-scope="{}">
              Devices
              <b-dropdown aria-role="list" class="is-pulled-right" position="is-bottom-left">
                <b-icon icon="dots-vertical" slot="trigger"></b-icon>
                <b-dropdown-item aria-role="listitem">Action</b-dropdown-item>
                <b-dropdown-item aria-role="listitem">Another action</b-dropdown-item>
                <b-dropdown-item aria-role="listitem">Something else</b-dropdown-item>
              </b-dropdown>
            </template>
          </b-menu-item>
          <b-menu-item icon="cash-multiple" label="Payments" disabled></b-menu-item>
        </b-menu-item>
        <b-menu-item icon="account" label="My Account">
          <b-menu-item label="Account data"></b-menu-item>
          <b-menu-item label="Addresses"></b-menu-item>
        </b-menu-item>
      </b-menu-list>
      <b-menu-list>
        <b-menu-item
          label="Expo"
          icon="link"
          tag="router-link"
          target="_blank"
          to="/expo">
        </b-menu-item>
      </b-menu-list>
      <b-menu-list label="Actions">
        <b-menu-item label="Logout"></b-menu-item>
      </b-menu-list>
    </b-menu>
  </section>
</template>

<script>
export default {
  name: 'Sidebar',
  data() {
    return {
      isActive: true
    }
  },
}
</script>

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
