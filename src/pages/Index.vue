<template>
  <q-page>
    <div class="text-center bgHome">
      <q-img src="home.png" width="15%" />
    </div>
    <q-tabs v-model="tab" align="justify" class="flex-center text-teal">
      <q-tab name="home" label="Home" />
      <q-tab name="aboutUs" label="About Us" />
      <q-tab name="indianRecruitment" label="Indian Recruitment" />
      <q-tab name="industries" label="Industries" />
      <q-tab name="insights" label="Insights" />
      <q-tab name="services" label="Services" />
    </q-tabs>
    <q-tab-panels v-model="tab" animated>
      <q-tab-panel name="home">
        <Home />
      </q-tab-panel>

      <q-tab-panel name="aboutUs">
        <AboutUs />
      </q-tab-panel>

      <q-tab-panel name="indianRecruitment">
        <IndianRecruitment />
      </q-tab-panel>
      <q-tab-panel name="industries">
        <Industries />
      </q-tab-panel>
      <q-tab-panel name="insights">
        <Insights />
      </q-tab-panel>
      <q-tab-panel name="services">
        <Services />
      </q-tab-panel>
    </q-tab-panels>
  </q-page>
</template>

<script>
import Home from "../components/Home.vue";
import AboutUs from "../components/AboutUs.vue";
import IndianRecruitment from "../components/IndianRecruitment.vue";
import Industries from "../components/Industries.vue";
import Insights from "../components/Insights.vue";
import Services from "../components/Services.vue";
export default {
  data() {
    return {
      tab: "home",
    };
  },
  components: {
    Home,
    AboutUs,
    Industries,
    Insights,
    Services,
    IndianRecruitment,
  },
};
</script>

<style>
.bgHome {
  background: radial-gradient(
    circle,
    rgba(108, 204, 207, 1) 2%,
    rgba(253, 254, 255, 1) 25%,
    rgba(69, 134, 211, 1) 87%
  );
}
</style>
