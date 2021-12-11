<template>
  <div id="app">
    <!-- header -->
    <header class="h-header">
      <Snowf
        :amount="150"
        :size="4"
        :speed="1.5"
        :wind="0"
        :opacity="0.8"
        :swing="1"
        :image="null"
        :zIndex="null"
        :resize="true"
        color="#fff"
      />
      <HeaderTop />
      <HeaderUnder />
    </header>
    <!-- /header -->
    <div class="module--spacing--small"></div>
    <Footer />
  </div>
</template>

<script>
import Snowf from "vue-snowf";
import HeaderTop from "./components/header/HeaderTop.vue";
import HeaderUnder from "./components/header/HeaderUnder.vue";

import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    Snowf,
    HeaderTop,
    HeaderUnder,
    Footer,
  },
};
</script>

<style>
.module--spacing--small {
  height: 20px;
}

.h-header {
  width: 100%;
  height: calc(75vh + 280px);
  position: relative;
}

</style>
