<template lang="html">
  <div class="nav">
    <router-link class="nav-item" v-for="link in links" :to="link.target" :key="link.id">
      {{link.text}}
    </router-link>
  </div>
</template>

<script>
import Router from '../router/index';

export default {
  name: 'navbar',
  Router,
  data() {
    return {
      links: [
        {
          text: 'Home',
          target: '/',
        },
        {
          text: 'Account',
          target: '/account',
        },

      ],
    };
  },
  components: {},

};
</script>

<style lang="css" scoped>
  .nav {
    height: 50px;
    margin-top: 1rem;
  }
  .nav-item {
    height: 50px;

    padding: 1rem;
    text-decoration: none;

    background-color: #2a4296;
    color: white;
  }
</style>
