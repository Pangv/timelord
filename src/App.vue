<template>
  <div id="app">
    <navbar id="navbar"></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from './components/Navbar';

export default {
  name: 'app',
  components: {
    Navbar,
  },
};
</script>

<style>
#app {

  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  border-radius: 0px;
}

button.btn.btn-primary {
  color: red;
  border-radius: 0px;
}

body {
  padding-top: 2rem;

}
</style>
