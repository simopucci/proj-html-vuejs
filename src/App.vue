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

        footerItems: {

          supportLinks: [
            {
              text: 'Contact Us',
              url: '#'
            },
            {
              text: 'Online Chat',
              url: '#'
            },
            {
              text: 'Whatsapp',
              url: '#'
            },
            {
              text: 'Telegram',
              url: '#'
            },
            {
              text: 'Snapchat',
              url: '#'
            },
          ],
          
          aboutLinks: [
            {
              text: 'About Us',
              url: '#'
            },
            {
              text: 'Blog',
              url: '#'
            },
            {
              text: 'Career',
              url: '#'
            },
            {
              text: 'Job',
              url: '#'
            },
            {
              text: 'In press',
              url: '#'
            },
          ],

          faqLinks: [
            {
              text: 'Account',
              url: '#'
            },
            {
              text: 'Order',
              url: '#'
            },
            {
              text: 'Delivery',
              url: '#'
            },
            {
              text: 'Payment',
              url: '#'
            },
            {
              text: 'Return',
              url: '#'
            },
          ],
        }
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
  <AppFooter
  :socials="headerItems.socials"
  :supportLinks="footerItems.supportLinks"
  :aboutLinks="footerItems.aboutLinks"
  :faqLinks="footerItems.faqLinks"></AppFooter>
</template>

<style lang="scss">
  @use './styles/general.scss';
</style>
