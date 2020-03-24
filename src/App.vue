<template>
  <div id="app">
    <b-container fluid class="p-0">
      <topNavbar class="" />
      <downNavbar class="bg-dark" />
    

    <b-container fluid  class="bg-primary main-content">

    <b-row class="bg-primary main-content">
      
      <b-col class="bg-danger col-md-9 offset-md-0">
        <b-row>
          <b-col cols="12"  lg="4" md="6" sm="12" v-for="a in 4" :key="a"><Books /></b-col>
        </b-row>
      </b-col>

      <b-col  class="col-md-3 offset-md-0 ">
        <b-row>
          <b-col cols="12" lg="12" md="6" sm="6" xs="12"> <asideTop /> </b-col>
          <b-col cols="12" lg="12" md="6" sm="6" xs="12"> <asideBottom /> </b-col>
        </b-row>
        
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
