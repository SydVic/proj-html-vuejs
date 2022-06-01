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
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container-general">
        <p>Enjoy the low price. We are tracking any intention of piracy.</p>
        <p>&copy; 2020 NEXGEN is Proudly Powered by <span class="txt-brand">Codings</span></p>
      </div>
      <div class="back-to-top">
        <a href="initial">
          <i class="fas fa-arrow-up"></i>
        </a>
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
  padding: $sections-padding;

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
      border-radius: 8px;
  
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
            color: $white;
          }
        }
      }
    }
  }
}

.footer-bottom {
  height: $footer-bottom-heigt;
  background-color: $black;
  color: $silver-sand;
  font-size: .9rem;
  position: relative;

  .container-general {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .back-to-top {
    color: $brand-primary-shadow;
    width: 45px;
    height: 45px;
    background-color: rgba(255, 255, 255, 0.2);
    position: absolute;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 1.3rem;
    text-align: center;
    line-height: 45px;
    border-radius: 50%;

    a {
      color: inherit;
    }
  }
}
</style>