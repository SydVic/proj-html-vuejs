<template>
  <section class="footer">
    <div class="footer-top">
      <div class="container-general">
        <div class="row">
          <div class="col-lg-3">
            <div class="content-wrapper">
              <div class="company-name">
                <span class="prename">{{companyObject.prename}}</span>
                <span class="name">{{companyObject.name}}</span>
              </div>
              <p class="paragraph">A functional HTML Template for Corporate & Business.</p>
              <ul class="company-contacts">
                <li>
                  <span class="icon-wrapper">
                    <i class="fas fa-phone-alt"></i>
                  </span>
                  <span class="text-wrapper">
                    {{ companyObject.phone }}
                  </span>
                </li>
                <li>
                  <span class="icon-wrapper">
                    <i class="fas fa-envelope"></i>
                  </span>
                  <span class="text-wrapper">
                    {{ companyObject.eMail }}
                  </span>
                </li>
                <li>
                  <span class="icon-wrapper">
                    <i class="fas fa-map-marker-alt"></i>
                  </span>
                  <span class="text-wrapper">
                    {{ companyObject.location }}
                  </span>
                </li>
              </ul>
              <div class="btn">
                <a href="" class="btn-secondary">get in touch</a>
              </div>
            </div>
          </div>
          <div v-for="(item, index) in footerItemsArray" :key="index" class="col-lg-3">
            <div class="content-wrapper">
              <div class="footer-card">
                <h2 class="txt-white">{{ footerItemsArray[index].title }}</h2>
                <ul class="footer-list">
                  <li v-for="(item, index) in footerItemsArray[index].items" :key="index">{{ item }}</li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="content-wrapper">

            </div>
          </div>
          <div class="col-lg-3">
            <div class="content-wrapper">

            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container-general">

      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppFooter",
  props: {
    companyObject: Object,
    footerItemsArray: Array,
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.footer-top {
  background-color: $sections-bg;
  padding: 8rem 0;

  ul.company-contacts {
    color: $silver-sand;

    li {
      margin-bottom: 1.5rem;

      span {
        display: inline-block;
      }

      span.icon-wrapper {
        margin-right: 1rem;
      }
    }
  }

  .content-wrapper {
    padding: 0 .7rem;

    .footer-card  {
      background-color: $card-bg;
      padding: 2rem 2.5rem 3rem 2.5rem;
  
      h2 {
        margin-bottom: 1.5rem;
      }
  
      ul.footer-list {
        color: $silver-sand;
  
        li {
          margin-bottom: .9rem;
          cursor: pointer;

          &::before {
            content:">";
            margin-right: .5rem;
          }

          &:hover {
            color: white;
          }
        }
      }
    }
  }
}

.footer-bottom {
  background-color: $black;

  /*test */
  height: 100px;
}
</style>