<template>
  <section class="feedback">
    <!-- FEEDBACK TITLE AND TEXT -->
    <div class="container-small mc-auto">
      <h3 class="title-small">customer testimonials</h3>
      <h2 class="title">
        <span class="title-normal txt-white">Trusted</span>
        <span class="title-highlighted txt-white">feedback</span>
      </h2>
      <p class="paragraph">We work intensively in search of ideals that can add up in the lives of our customers. Thi is what moves us and we are grateful for the recognition.</p>
    </div>
    <!-- /FEEDBACK TITLE AND TEXT -->

    <!-- CONTAINER WIDTH 60% -->
    <div class="container-general">
      <!-- ROW -->
      <div class="row">
        <!-- COL-4 -->
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="feedback-card">
            <div class="feedback-img">
              <img src="../assets/img/logo-1.png" alt="">
            </div>
            <p class="paragraph">Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pallentesque.</p>
            <p class="paragraph strict">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
              <div class="icon-wrapper">
              <i class="fas fa-quote-right"></i>
            </div>
          </div>
          <!-- /CARD -->
        </div>
        <!-- /COL-4 -->

        <!-- COL-4 -->
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="feedback-card mc-auto">
            <div class="feedback-img">
              <img src="../assets/img/logo-2.png" alt="">
            </div>
            <p class="paragraph">Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pallentesque.</p>
            <p class="paragraph strict">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
              <div class="icon-wrapper">
              <i class="fas fa-quote-right"></i>
            </div>
          </div>
          <!-- /CARD -->
        </div>
        <!-- /COL-4 -->

        <!-- COL-4 -->
        <div class="col-lg-4">
          <!-- CARD -->
          <div class="feedback-card ml-auto">
            <div class="feedback-img">
              <img src="../assets/img/logo-3.png" alt="">
            </div>
            <p class="paragraph">Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pallentesque.</p>
            <p class="paragraph strict">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            <div class="icon-wrapper">
              <i class="fas fa-quote-right"></i>
            </div>
          </div>
          <!-- /CARD -->
        </div>
        <!-- /COL-4 -->
      </div>
      <!-- /ROW -->
    </div>
    <!-- /CONTAINER WIDTH 60% -->
  </section>
</template>

<script>
export default {
  name: "MainFeedback",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.feedback {
  padding: $sections-padding;
  background-color: $sections-bg;

  .container-small {
    text-align: center;

    .title-normal {
      padding-right: .5rem;
    }
  
    .paragraph {
      margin-bottom: 0;
    }
  }

  .feedback-card {
    width: 95%;
    background-color: $card-bg;
    padding: 2.5rem 2rem;
    border-radius: 10px;
    margin-top: 3rem;
    position: relative;

    .paragraph {
      margin: .5rem 0 .5rem 0;

      &.strict {
        display: inline-block;
        width: 80%;
      }
    }

    .feedback-img {
      width: 40%;
      height: 40px;

      img {
        filter: invert(100%);
      }
    }

    .icon-wrapper {
      font-size: 1.5rem;
      color: #47474c;
      display: inline-block;
      position: absolute;
      bottom: 10%;
      right: 5%;
    }
  }
}
</style>