<template>
  <div id="app">
    <div style="min-height:610px;">
      <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand>Youtube To MP3 Converter</b-navbar-brand>
      </b-navbar>
      <Home />
    </div>
    <div class="fluid-container footer">
      <p class="text-center">Copyright</p>
    </div>
  </div>
</template>

<script>
import Home from './components/Home.vue';
import Vue from 'vue';
import BootstrapVue from 'bootstrap-vue';

Vue.use(BootstrapVue);

export default {
  name: 'app',
  components: {
    Home
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
.fluid-container.footer {
  margin-bottom: 0px;
}
</style>
