<template>
  <div id="app">
    <CxHeader />
    <CxHero />
    <CxServices />
    <CxAbout />
    <CxTestimonials />
    <CxContactForm />
  </div>
</template>

<script>
import CxHeader from "./components/CxHeader.vue";
import CxHero from "./components/CxHero.vue";
import CxServices from "./components/CxServices.vue";
import CxAbout from "./components/CxAbout.vue";
import CxTestimonials from "./components/CxTestimonials.vue";
import CxContactForm from "./components/CxContactForm.vue";

export default {
  components: {
    CxHeader,
    CxHero,
    CxServices,
    CxAbout,
    CxTestimonials,
    CxContactForm,
  },
};
</script>
