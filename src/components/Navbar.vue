<template lang="html">
  <ul class="nav nav-pills">
    <li role="presentation" v-for="link in links" >
      <router-link class="btn btn-primary" :to="link.target" :key="link.id">
        {{link.text}}
      </router-link>
    </li>
  </ul>
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
          text: 'Mein Profil',
          target: '/profil',
        },

      ],
    };
  },
  components: {},

};
</script>

<style lang="css" scoped>
  ul {
    display: inline-block;
    margin-bottom: 2rem;
  }
  .btn-primary:hover, .btn-primary:active, .btn-primary:focus {
      color: black;
  }
</style>
