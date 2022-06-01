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
            </div>
          </div>
          <div class="col-lg-3">
            <div class="content-wrapper">
              <div class="company-name">
                <span class="prename">{{companyObject.prename}}</span>
                <span class="name">{{companyObject.name}}</span>
              </div>
              <p class="paragraph">A functional HTML Template for Corporate & Business.</p>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="content-wrapper">
              <div class="company-name">
                <span class="prename">{{companyObject.prename}}</span>
                <span class="name">{{companyObject.name}}</span>
              </div>
              <p class="paragraph">A functional HTML Template for Corporate & Business.</p>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="content-wrapper">
              <div class="company-name">
                <span class="prename">{{companyObject.prename}}</span>
                <span class="name">{{companyObject.name}}</span>
              </div>
              <p class="paragraph">A functional HTML Template for Corporate & Business.</p>
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
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.footer-top {
  background-color: $shark;
  padding: 8rem 0;

  /*test */
  height: 800px;
}

.footer-bottom {
  background-color: $black;

  /*test */
  height: 100px;
}
</style>