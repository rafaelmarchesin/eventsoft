<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" app class="primary">
      <h1>Teste</h1>
      <p>Teste Estamos aqui!</p>
    </v-navigation-drawer>

    <v-app-bar app color="primary" dark>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>EventSoft</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <Home />

      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
    </v-main>

    <v-content> Conteúdo </v-content>

    <v-footer app> Rodapé </v-footer>
  </v-app>
</template>

<script>
import Home from "./components/Home.vue";

export default {
  name: "App",

  components: {
    Home,
  },

  data: () => ({
    drawer: true,
  }),
};
</script>
