<template>
  <div id="app">
    <dc_header/>
    <ContentComponent :cards="fumetti"/>
    <blue_nav/>
    <dc_main/>
    <dc_footer/>
  </div>
</template>

<script>
import dc_header from './components/header.vue'
import ContentComponent from './components/ContentComponent.vue'
import blue_nav from './components/blue_nav.vue'
import dc_main from './components/dc_main.vue'
import dc_footer from './components/dc_footer.vue'

import {fumetti} from './assets/img/data/data_content'
// con le parentesi graffe importa solo un dato, senza importo l'intero file

export default {
  name: 'App',
  data() {
    return {
      fumetti
    }
  },
  components: {
    dc_header,
    ContentComponent,
    blue_nav,
    dc_main,
    dc_footer
  }
  
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');
body {
  // reset css
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}
a{
  text-decoration: none;
  color: #fff;
}
</style>
