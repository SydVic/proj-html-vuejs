<template>
  <div id="app">
    <AppHeader :companyObject="companyInfo" :navItemsArray="navItems"/>
    <AppMain />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import "@fontsource/aileron";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  data: function() {
    return {
      companyInfo: {
        prename: 'nex',
        name: 'gen',
        phone: '+1 (305) 1234-5678',
        eMail: 'hello@example.com',
        openingDay: 'Mon',
        closingDay: 'Sat',
        openingHour: '9:00',
        closingHour: '18:00',
        socialContacts: [ 
          {
            prefix: 'fab',
            social: 'fa-facebook'
          },
          {
            prefix: 'fab',
            social: 'fa-twitter'
          },
          {
            prefix: 'fab',
            social: 'fa-linkedin-in'
          },
        ]
      },
      navItems: [
        'home',
        'about',
        'services',
        'process',
        'testimonials',
      ]
    }
  }
}
</script>

<style lang="scss">
@import "./style/framework-12cols.scss";
@import "./style/common.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";


</style>
