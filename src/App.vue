<template>
  <v-app>
    <div class="app">
      <router-link :to="{ name: 'Home' }"></router-link>
      <router-link :to="{ name: 'About' }"></router-link>
    </div>
    <router-view />
  </v-app>
</template>

<script>

export default {
  name: 'App',
};
</script>
