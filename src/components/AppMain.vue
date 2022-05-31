<template>
  <main class="main">
    <MainWhoWeAre />
    <MainServices />
    <MainLogistics />
  </main>
</template>

<script>
import MainWhoWeAre from "./MainWhoWeAre.vue";
import MainServices from "./MainServices.vue";
import MainLogistics from "./MainLogistics.vue";

export default {
  name: "AppMain",
  components: {
    MainWhoWeAre,
    MainServices,
    MainLogistics,
  }
}
</script>

<style lang="scss" scoped>

</style>