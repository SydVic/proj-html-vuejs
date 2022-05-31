<template>
  <section class="logistical">
    <div class="container-small mc-auto">
      <h3 class="title-small">how it works in practice</h3>
      <h2 class="title">
        <span class="title-highlighted txt-brand">Logistical</span>
        <span class="title-normal">Procedure</span>
      </h2>
      <p class="paragraph">We work with innovative methodoligies to ensure that the entire delivery process is done from start to finish as planned.</p>
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
}
</style>