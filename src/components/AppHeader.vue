<template>
  <!-- HAEDER WIDTH 100% -->
  <section class="header container-fluid">
    <!-- HEADER TOP WIDTH 100% -->
    <div class="header__top">
      <!-- COMPANY INFO WRAPPER WIDTH 60% -->
      <div class="company-info-wrapper container-general">
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
              <i class="fas fa-phone-alt"></i>
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
      <div class="container-general">
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

        <!-- JUMBOTRON TEXT -->
        <div class="jumbotron-text">
          <div class="row">
            <div class="col-lg-5">
              <h3 class="title-small">logistics services</h3>
              <h2>cargo transport</h2>
              <p>Fractional or exclusive road cargo transportation to all regions, with small, medium and large vehicles.</p>
              <div class="jumbotron-cta">
                <div class="btn">
                  <a class="btn-primary">get in touch</a>
                </div>
                <div class="btn">
                  <a class="btn-secondary">read more</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- /JUMBOTRON TEXT -->
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
  position: relative;

  &::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,.6);
  }

  .nav-wrapper {
    padding-top: 2.5rem;
    display: flex;
    justify-content: space-between;
    font-size: 1.1rem;
    font-weight: 100;
    position: relative;

    .company-name {
      text-transform: uppercase;
      font-size: 1.5rem;
      font-weight: bold;
      letter-spacing: 3px;
  
      .prename {
        color: $brand-primary;
        background-color: $brand-primary-shadow;
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
        align-items: center;

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

  .jumbotron-text {
    padding: 10rem 0 15rem 0;
    position: relative;

    h2 {
      color: $white;
      text-transform: uppercase;
      font-size: 4rem;
      font-weight: 900;
      line-height: 5rem;
    }

    p {
      color: $silver-sand;
      font-size: 1.2rem;
      line-height: 1.8rem;
      margin: 1.5rem 0 3rem 0;
    }

    .jumbotron-cta {
      display: flex;

      .btn-primary {
        margin-right: 1.5rem;
      }
    }
  }
}
</style>