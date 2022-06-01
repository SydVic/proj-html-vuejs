<template>
  <section class="results">
    <!-- CONTAINER WIDTH60% -->
    <div class="container-general">
      <!-- TITLE -->
      <h3 class="title-small">what are we doing</h3>
      <h2 class="title">
        <span class="title-highlighted txt-white">Results</span>
        <span class="title-normal txt-white"> in Numbers</span>
      </h2>
      <!-- /TITLE -->

      <!-- ROW -->
      <div class="row">
        <!-- COL-3 -->
        <div class="col-lg-3">
          <div class="txt-brand">128</div>
          <h2 class="txt-white">Certifications</h2>
        </div>
        <!-- /COL-3 -->

        <!-- COL-3 -->
        <div class="col-lg-3">
          <div class="txt-brand">230</div>
          <h2 class="txt-white">Employees</h2>
        </div>
        <!-- /COL-3 -->

        <!-- COL-3 -->
        <div class="col-lg-3">
          <div class="txt-brand">517</div>
          <h2 class="txt-white">Customers</h2>
        </div>
        <!-- /COL-3 -->

        <!-- COL-3 -->
        <div class="col-lg-3">
          <div class="txt-brand">94</div>
          <h2 class="txt-white">Countries Served</h2>
        </div>
        <!-- /COL-3 -->
      </div>
      <!-- /ROW -->
    </div>
    <!-- /CONTAINER WIDTH60% -->
  </section>
</template>

<script>
export default {
  name: "MainResults",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.results {
  background-image: $results-jumbotron-img;
  background-position: center;
  padding: $sections-padding;
  position: relative;

    &::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,.4);
  }

  .container-general {
    text-align: center;
    position: relative;

    .txt-brand {
      font-size: 2rem;
      font-weight: 900;
      margin: 4rem 0 1rem 0;
    }
  }
}
</style>