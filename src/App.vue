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
    'v-main': Main
  }
}
</script>

<style lang="sass">
// 所有的变量声明
// 头部栏的高度
$headerHeight: 60px


html,
body
  width: 100%
  height: 100%
  margin: 0
  padding: 0

#app
  height: inherit
  .page-wrapper
    height: inherit
    .page-content
      position: absolute
      top: $headerHeight
      bottom: 0
      width: 100%
      background: #333


// #app {
//   font-family: 'Avenir', Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
