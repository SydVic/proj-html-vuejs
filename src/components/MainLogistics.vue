<template>
  <section class="logistical">
    <div class="container-small mc-auto">
      <h3 class="title-small">how it works in practice</h3>
      <h2 class="title">
        <span class="title-highlighted txt-brand">Logistical</span>
        <span class="title-normal"> Procedure</span>
      </h2>
      <p class="paragraph">We work with innovative methodoligies to ensure that the entire delivery process is done from start to finish as planned.</p>
    </div>
    <div class="logistical-steps">
      <div class="line"></div>
      <div class="container-large mc-auto">
        <div class="row">
          <div class="col">
            <div class="step-wrapper">
              <div class="rounded-number">01</div>
              <h2>Collection of information</h2>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur.</p>
            </div>
          </div>
          <div class="col">
            <div class="step-wrapper">
              <div class="rounded-number">02</div>
              <h2>Service Invoice Sending</h2>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur.</p>
            </div>
          </div>
          <div class="col">
            <div class="step-wrapper">
              <div class="rounded-number">03</div>
              <h2>Withdrawal of Cargo</h2>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur.</p>
            </div>
          </div>
          <div class="col">
            <div class="step-wrapper">
              <div class="rounded-number">04</div>
              <h2>Transport Customer Order</h2>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur.</p>
            </div>
          </div>
          <div class="col">
            <div class="step-wrapper">
              <div class="rounded-number">05</div>
              <h2>Successful Delivery</h2>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainLogistics"
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.logistical {
  background-color: #eef4ed;
  padding: 8rem 0;

  .container-small {
    text-align: center;

    .paragraph {
      color: $mid-gray;
    }
  }

  .logistical-steps {
    padding-top: 3rem;

    .line {
      height: 5px;
      width: 100%;
      background-color: $brand-primary-shadow;
    }

    .container-large {
      text-align: center;
      position: relative;

      .col {
        width: 16%;

        .step-wrapper {
          padding: 0 3rem;
          margin-top: - 1.5rem;

          .rounded-number {
            color: $brand-primary;
            background-color: #daeced;
            font-size: 1.3rem;
            font-weight: 700;
            padding: .6rem;
            display: inline-block;
            border-radius: 50%;
          }

          h2 {
            margin-top: 1.5rem;
          }

          p {
            color: $mid-gray;
          }
        }
      }
    }
  }
}
</style>