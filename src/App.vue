<template>
  <v-app>
    <Home/>
    <router-view></router-view>
  </v-app>
</template>

<script>
import Home from './views/Home'

export default {
  name: 'App',
  components: {
    Home
  }
};
</script>
