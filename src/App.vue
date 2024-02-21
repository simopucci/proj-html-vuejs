<script>
  import { store } from './store';

  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    data() {
      return {
        store,

        headerItems: {

          socials: [
            {
              name: 'fa-brands fa-square-facebook',
              url: '#',
              color: 'color: #0000ce'
            },
            {
              name: 'fa-brands fa-square-pinterest',
              url: '#',
              color: 'color: #a93d3d'
            },
            {
              name: 'fa-brands fa-square-x-twitter',
              url: '#',
              color: 'color: lightblue'
            },
            {
              name: 'fa-brands fa-linkedin',
              url: '#',
              color: 'color: #3131ce'
            },
            {
              name: 'fa-brands fa-square-instagram',
              url: '#',
              color: 'color: #920292'
            },
          ],

          headerLinks: [
            {
                text: 'Home',
                url: '#'
            },
            {
                text: 'About',
                url: '#'
            },
            {
                text: 'Services',
                url: '#'
            },
            {
                text: 'Training',
                url: '#'
            },
            {
                text: 'Blogs',
                url: '#'
            },
          ],

          logo: '../assets/img/logo.png'
        },

      };
    },

    components: { AppHeader, AppMain, AppFooter }
  }

</script>

<template>
  <AppHeader
  :headerLinks="headerItems.headerLinks"
  :logoPath="headerItems.logo"
  :socials="headerItems.socials">
  </AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
  @use './styles/general.scss';
</style>
