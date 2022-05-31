<template>
  <main class="main">
    <MainWhoWeAre />
    <MainServices />
    <MainLogistics />
    <MainResults />
    <MainFeedback />
  </main>
</template>

<script>
import MainWhoWeAre from "./MainWhoWeAre.vue";
import MainServices from "./MainServices.vue";
import MainLogistics from "./MainLogistics.vue";
import MainResults from "./MainResults.vue";
import MainFeedback from "./MainFeedback.vue";

export default {
  name: "AppMain",
  components: {
    MainWhoWeAre,
    MainServices,
    MainLogistics,
    MainResults,
    MainFeedback,
  }
}
</script>

<style lang="scss" scoped>

</style>