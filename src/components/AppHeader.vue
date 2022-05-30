<template>
  <!-- HAEDER WIDTH 100% -->
  <section class="header container-fluid">
    <!-- HEADER TOP WIDTH 100% -->
    <div class="header__top">
      <!-- COMPANY INFO WRAPPER WIDTH 60% -->
      <div class="company-info-wrapper container-small">
        <!-- OPENING DAYS AND HORURS -->
        <div class="company-hours">
          <span class="clock-icon">
            <i class="fas fa-clock"></i>
          </span>
          <span>Open Hours: {{ companyObject.openingDay }} - {{ companyObject.closingDay }} - {{ companyObject.openingHour }} - {{ companyObject.closingHour }}</span>
        </div>
        <!-- /OPENING DAYS AND HORURS -->

        <!-- CONTACTS -->
        <div class="company-contacts">
          <!-- PHONE ADN MAIL -->
          <span class="company-phone-number">
            <span class="phone-icon">
              <i class="fas fa-phone"></i>
            </span>
            {{ companyObject.phone }}
          </span>
          <span class="company-mail">
            <span class="envelope-icon">
              <i class="fas fa-envelope"></i>
            </span>
            {{ companyObject.eMail }}
          </span>
          <!-- /PHONE ADN MAIL -->  

          <!-- SOCIAL CONTACTS -->
          <ul class=social-list>
            <li v-for="(item, index) in companyObject.socialContacts" :key="index">
              <a href="">
                <i :class="`${item.prefix} ${item.social}`"></i>
              </a>
            </li>
          </ul>
          <!-- /SOCIAL CONTACTS -->
        </div>
        <!-- /CONTACTS -->
      </div>
      <!-- /COMPANY INFO WRAPPER WIDTH 60% -->
    </div>
    <!-- /HEADER TOP WIDTH 100% -->

    <!-- HEADER BOTTOM WIDTH 100% -->
    <div class="header__bottom">
      <!-- JUMBOTRON WRAPPER WIDTH 60% -->
      <div class="container-small">
        <!-- NAV WRAPPER -->
        <div class="nav-wrapper">
          <!-- COMPANY NAME -->
          <div class="company-name">
            <span class="prename">{{companyObject.prename}}</span>
            <span class="name">{{companyObject.name}}</span>
          </div>
          <!-- /COMPANY NAME -->

          <!-- NAV ITEMS -->
          <div class="nav-items">
            <ul>
              <li v-for="(item, index) in navItemsArray" :key="index">
                <a href="">{{ item }}</a>
              </li>
              <li>
                <a href="">
                  <i class="far fa-user"></i>
                </a>
              </li>
              <li>
                <a class="btn-primary" href="">get in touch</a>
              </li>
            </ul>
          </div>
          <!-- /NAV ITEMS -->
        </div>
        <!-- /NAV WRAPPER -->
      </div>
      <!-- /JUMBOTRON WRAPPER WIDTH 60% -->
    </div>
    <!-- /HEADER BOTTOM WIDTH 100% -->
  </section>
  <!-- /HAEDER WIDTH 100% -->
</template>

<script>
export default {
  name: "AppHeader",
  props: {
    companyObject: Object,
    navItemsArray: Array,
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.header__top {
  color: $silver-sand;
  font-weight: 100;
  background-color: $header-top-bg;
  height: $header-top-height;
  display: flex;
  align-items: center;

  .company-info-wrapper {
  display: flex;
  justify-content: space-between;

    .clock-icon {
      margin-right: .5rem;
    }

    .company-contacts {
      display: flex;

      .company-phone-number {
        margin-right: 2rem;

        .phone-icon {
          margin-right: .3rem;
        }
      }

      .company-mail {

        .envelope-icon {
          margin-right: .3rem;
        }
      }

      ul.social-list {
        display: flex;

        li {
          margin-left: 2rem;

          a {
            color: inherit;
          }
        }
      }
    }
  }
}
  
.header__bottom {
  background-image: $header-jumbotron-img;

  .nav-wrapper {
    padding: 2.5rem 0 5rem 0;
    display: flex;
    justify-content: space-between;

    .company-name {
      text-transform: uppercase;
      font-size: 1.5rem;
      font-weight: bold;
      letter-spacing: 3px;
  
      .prename {
        color: $brand-primary;
        background-color: rgba(22, 146, 142, .3);
        padding: .5rem .2rem .5rem 1.5rem;
        border-top-left-radius: 30px;
        border-bottom-left-radius: 30px;
      }
      .name {
        color: $silver-sand;
        padding-left: .2rem;
      }
    }

    .nav-items {

      ul {
        display: flex;

        li {
          margin-left: 1.5rem;
          text-transform: uppercase;
          color: $white;

          a {
            color: inherit;
          }
        }
      }
    }
  }
}


</style>