<template>
  <div id="app">
    <b-container fluid class="p-0">
      <topNavbar class="" />
      <downNavbar class="bg-dark" />
    

    <b-container fluid  class="bg-primary main-content">
    <b-row class="bg-primary main-content">
      <b-col cols="9" class="bg-danger">
        <Books />
      </b-col>
      <b-col cols="3" class="d-flex d-flex-column">
        <asideTop />
        <asideBottom />
      </b-col>
    </b-row>
    </b-container>

  <!-- 
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about/10">About</router-link>
    </div>
    <router-view />
  </div>-->
    </b-container>
  </div>

</template>

<script>
import topNavbar from "./components/topNavbar";
import downNavbar from "./components/downNavbar";

import asideTop from "./components/asideTop";
import asideBottom from "./components/asideBottom";

import Books from './components/Books'

export default {
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: {
    topNavbar,
    downNavbar,
    asideTop,
    asideBottom,
    Books
  }
};
</script>

<style lang="scss" scoped>
#app{
    box-sizing: border-box;
  .main{
  }
    .main-content {

      min-height: 85vh;
    }
}
</style>
