<template>
  <span>
    <Header />
    <v-container>
      <Timeline />
    </v-container>
    <Banner />
    <More />
    <Footer/>
  </span>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
};
</script>
