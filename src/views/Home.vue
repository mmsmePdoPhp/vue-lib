<template>
  <div class="home">
    <topNavbar msg="Welcome to Your Vue.js App"/>
 
    

    
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->


  </div>
</template>

<script>
// @ is an alias to /src
import topNavbar from '@/components/topNavbar.vue'

export default {
  name: 'Home',
  components: {
    topNavbar
  }
}
</script>
