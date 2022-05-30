<template>
  <!-- HAEDER WIDTH 100% -->
  <section class="header container-fluid">
    <!-- HEADER TOP WIDTH 100% -->
    <div class="header__top">
      <!-- COMPANY INFO WRAPPER WIDTH 60% -->
      <div class="company-info-wrapper container-small">
        <!-- OPENING DAYS AND HORURS -->
        <div class="company-hours">
          <i class="fas fa-clock"></i>
          <span>Open Hours: {{ companyObject.openingDay }} - {{ companyObject.closingDay }} - {{ companyObject.openingHour }} - {{ companyObject.closingHour }}</span>
        </div>
        <!-- /OPENING DAYS AND HORURS -->

        <!-- CONTACTS -->
        <div class="company-contacts">
          <!-- PHONE ADN MAIL -->
          <span class="company-phone-number">
            <i class="fas fa-phone-alt"></i>
            {{ companyObject.phone }}
          </span>
          <span class="company-phone-number">
            <i class="fas fa-envelope"></i>
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
        </div>
        <!-- /CONTACTS -->
      </div>
      <!-- /COMPANY INFO WRAPPER WIDTH 60% -->
    </div>
    <!-- /HEADER TOP WIDTH 100% -->

    <!-- HEADER BOTTOM WIDTH 100% -->
    <div class="header__bottom">

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
  color: #bcbdbd;
  background-color: $header-top-bg;
  height: $header-top-height;
  display: flex;
  align-items: center;

  .company-info-wrapper {
  display: flex;
  justify-content: space-between;

    .company-contacts {
      display: flex;

      ul.social-list {
        list-style: none;
        display: flex;
      }
    }
  }
}
  
.header__bottom {
  background-image: $header-jumbotron-img;
  
  /*test*/
  height: 800px;
}


</style>