<template>
  <v-app>
    <v-app-bar app color="transparent" hide-on-scroll>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>
        Lo-Fi - ローファイ
      </v-toolbar-title>
    </v-app-bar>
    <v-main>
      <Home/>
    </v-main>
  </v-app>
</template>

<script>
import Home from './components/Home'

export default {
  name: 'App',
  components: {
    Home
  },
  data: () => ({
    //
  })
}
</script>
