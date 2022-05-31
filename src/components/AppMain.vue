<template>
  <main class="main">
    <MainWhoWeAre />
    <MainServices />
    <MainLogistics />
    <MainResults />
    <MainFeedback />
    <MainContactUs />
  </main>
</template>

<script>
import MainWhoWeAre from "./MainWhoWeAre.vue";
import MainServices from "./MainServices.vue";
import MainLogistics from "./MainLogistics.vue";
import MainResults from "./MainResults.vue";
import MainFeedback from "./MainFeedback.vue";
import MainContactUs from "./MainContactUs.vue";

export default {
  name: "AppMain",
  components: {
    MainWhoWeAre,
    MainServices,
    MainLogistics,
    MainResults,
    MainFeedback,
    MainContactUs,
  }
}
</script>

<style lang="scss" scoped>

</style>