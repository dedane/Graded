<template>
  <nav>
    <v-toolbar flat app color="cyan darken-1">
      <v-toolbar-side-icon color="cyan darken-1" @click="drawer = !drawer" />
      <v-toolbar-title class="text-uppercase white--text">
        <span class="font-weight-light">School System</span>
      </v-toolbar-title>
      <v-spacer />
      <v-icon large color="teal darken-2">
        email
      </v-icon>
    </v-toolbar>

    <v-navigation-drawer v-model="drawer" app class="purple">
      <v-list>
        <v-list-tile v-for="link in links" :key="link.text" router :to="link.route">
          <v-list-tile-action>
            <v-icon class="white--text">
              {{ link.icon }}
            </v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="white--text">
              {{ link.text }}
            </v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>
<script>
export default {
  data() {
    return {
      drawer: false,
      links: [
        { icon: 'dashboard', text: 'Dashboard', route: '/' },
        { icon: 'person', text: 'Teachers', route: '/' },
        { icon: 'people', text: 'Students', route: '/' }
      ]
    }
  }
}
</script>
