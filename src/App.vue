<template>
  <div id="app">
    <AppHeader :companyObject="companyInfo" :navItemsArray="headerNavItems"/>
    <main class="main">
      <MainWhoWeAre />
      <MainServices />
      <MainLogistics />
      <MainResults />
      <MainFeedback />
      <MainContactUs :companyObject="companyInfo" />
    </main>
    <AppFooter :companyObject="companyInfo" :footerItemsArray="footerNavItems" />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import MainWhoWeAre from "./components/MainWhoWeAre.vue";
import MainServices from "./components/MainServices.vue";
import MainLogistics from "./components/MainLogistics.vue";
import MainResults from "./components/MainResults.vue";
import MainFeedback from "./components/MainFeedback.vue";
import MainContactUs from "./components/MainContactUs.vue";
import AppFooter from "./components/AppFooter.vue";
import "@fontsource/aileron";

export default {
  name: 'App',
  components: {
    AppHeader,
    MainWhoWeAre,
    MainServices,
    MainLogistics,
    MainResults,
    MainFeedback,
    MainContactUs,
    AppFooter,
  },
  data: function() {
    return {
      companyInfo: {
        prename: 'nex',
        name: 'gen',
        phone: '+1 (305) 1234-5678',
        eMail: 'hello@example.com',
        location: 'Main Avenue, 987',
        openingDay: 'Mon',
        closingDay: 'Sat',
        openingHour: '9:00',
        closingHour: '18:00',
        socialContacts: [ 
          {
            prefix: 'fab',
            social: 'fa-facebook-f'
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
      headerNavItems: [
        'home',
        'about',
        'services',
        'process',
        'testimonials',
      ],
      footerNavItems: [
        {
          title: 'About',
          items: [
            'The Company',
            'Insitutional',
            'Social & Events',
            'Innovation',
            'Environment',
            'Technology',
          ]
        },
        {
          title: 'Transport',
          items: [
            'Industrialized',
            'Chemicals',
            'Packaged Liquids',
            'Construction',
            'Laminated Wood',
            'And others',
          ]
        },
        {
          title: 'Support',
          items: [
            'Responsibility',
            'Terms of Use',
            'About Cookies',
            'Privacy Policy',
            'Accessibility',
            'Information',
          ]
        }
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
