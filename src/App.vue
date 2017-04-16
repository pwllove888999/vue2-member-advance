<template>
  <div id="app">
    <div class="page-wrapper">
      <v-header></v-header>
      <div class="page-content">
        <v-menu></v-menu>
        <v-main></v-main>
      </div>
    </div>

  </div>
</template>

<script>
import Header from './components/header/header.vue'
import Menu from './components/menu/menu.vue'
import Main from './components/main/main.vue'
export default {
  data () {
    return {

    }
  },
  components: {
    'v-header': Header,
    'v-menu': Menu,
    'v-main': Main,
  }
}
</script>

<style>
/*#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}*/
</style>
