<template>
  <main class="main">
    <MainWhoWeAre />
    <MainServices />
  </main>
</template>

<script>
import MainWhoWeAre from "./MainWhoWeAre.vue";
import MainServices from "./MainServices.vue";

export default {
  name: "AppMain",
  components: {
    MainWhoWeAre,
    MainServices,
  }
}
</script>

<style lang="scss" scoped>

</style>