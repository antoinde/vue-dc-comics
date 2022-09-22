<template>
  <div id="app">
    <dc_header/>
    <black_header/>
    <blue_nav/>
    <dc_main/>
    <dc_footer/>
  </div>
</template>

<script>
import dc_header from './components/header.vue'
import black_header from './components/header2.vue'
import blue_nav from './components/blue_nav.vue'
import dc_main from './components/dc_main.vue'
import dc_footer from './components/dc_footer.vue'

export default {
  name: 'App',
  components: {
    dc_header,
    black_header,
    blue_nav,
    dc_main,
    dc_footer
  }
}
</script>

<style lang="scss">
body {
  // reset css
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
