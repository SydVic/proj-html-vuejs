<template>
  <section class="services">
    <!-- CONTAINER WIDTH 60% -->
    <div class="container-general">
      <!-- SERVICES TITLE AND TEXT -->
      <div class="row">
        <div class="col-lg-8">
          <h3 class="title-small">road transport</h3>
          <h2 class="title">
            <span class="title-normal txt-white">Main</span>
            <span class="title-highlighted txt-white">Services</span>
          </h2>
          <p class="paragraph">With all of this expertise and capability comes an unrivalled commitment to customer service. We will work hard to understand your needs in order to develop a productive, long-term partnership.</p>
        </div>
        <div class="col-lg-4">
          <div class="wrapper-flex">
            <div class="btn">
              <a class="btn-secondary">see all</a>
            </div>
          </div>
        </div>
      </div>
      <!-- /SERVICES TITLE AND TEXT -->

      <!-- SERVICES CARDS -->
      <div class="row">
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="services-card">
            <div class="icon-wrapper">
              <div class="card-icon">
                <i class="fas fa-truck-loading"></i>
              </div>
              <div class="arrow-icon">
                <i class="fas fa-arrow-right"></i>
              </div>
            </div>
            <h2 class="txt-white">Technology</h2>
            <p class="paragraph">We are continually focused on developing technology solutions adapted to our client's needs.</p>
          </div>
          <!-- /CARD -->
        </div>
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="services-card mc-auto">
            <div class="icon-wrapper">
              <div class="card-icon">
                <i class="fas fa-temperature-low"></i>
              </div>
              <div class="arrow-icon">
                <i class="fas fa-arrow-right"></i>
              </div>
            </div>
            <h2 class="txt-white">Refeer Cargo</h2>
            <p class="paragraph">Regular and frequent monitoring from the receipt of the loaded container to final destination.</p>
          </div>
          <!-- /CARD -->
        </div>
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="services-card ml-auto">
            <div class="icon-wrapper">
              <div class="card-icon">
                <i class="fas fa-boxes"></i>
              </div>
              <div class="arrow-icon">
                <i class="fas fa-arrow-right"></i>
              </div>
            </div>
            <h2 class="txt-white">Dry Cargo</h2>
            <p class="paragraph">We work with most of types of dry cargo, from valuable cargo to the most dangerous requiring care.</p>
          </div>
          <!-- /CARD -->
        </div>
      </div>
      <!-- /SERVICES CARDS -->
    </div>
    <!-- /CONTAINER WIDTH 60% -->
  </section>
</template>

<script>
export default {
  name: "MainServices",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.services {
  padding: 8rem 0;
  background-color: $sections-bg;

  .title-normal {
    padding-right: .5rem;
  }

  .paragraph {
    margin-bottom: 0;
  }

  .wrapper-flex {
    height: 100%;
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
  }
  
  .services-card {
    width: 95%;
    background-color: #19191f;
    padding: 2.5rem 2rem;
    border-radius: 10px;
    margin-top: 3rem;

    .icon-wrapper {
      display: flex;
      justify-content: space-between;

      .card-icon {
        background-color: $brand-primary-shadow;
        color: $brand-primary;
        font-size: 1.7rem;
        padding: 1rem;
        border-radius: 50%;
      }

      .arrow-icon {
        color: $brand-primary-shadow;
        font-size: 1.5rem;
      }
    }

    h2 {
      margin-top: 1.5rem;
    }
  }
}
</style>