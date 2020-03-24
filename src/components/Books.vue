<template>
 
<div class="my-2">
  <b-card
    style="max-width: 20rem;"
    img-top
  >
    <template v-slot:header>
      <b-card-img src="https://placekitten.com/480/210" alt="Image" bottom></b-card-img>
    </template>

    <b-card-body>
      <b-card-title>Eloquent Javascript</b-card-title>
      <b-card-sub-title class="mb-2">
        <p class="m-2">write by: <strong>john donson</strong></p>
        <p class="m-2">pages:<b>256</b> </p>
        </b-card-sub-title>
      <b-card-text class="my-2">
        Some quick example text to build on the card title and make up the bulk of the card's
        content.
      </b-card-text>
    </b-card-body>


    <b-card-footer>
      <b-row>
        <b-col>$ 23</b-col>
        <b-col>
          <!-- <b-icon icon="heart"></b-icon> -->
          <!-- <b-icon icon="heart-fill"></b-icon> -->
          
          <b-icon icon="heart-half"></b-icon>
        </b-col>
        <b-col>
          <b-icon icon="chat-quote"></b-icon>
        </b-col>
        <b-col>
          <b-icon icon="arrow-down"></b-icon>24
        </b-col>
      </b-row>

    </b-card-footer>

  </b-card>
</div>
</template>

<script>
export default {};
</script>


<style lang="scss" scoped>
.card-body{
  padding-top:0px;
  padding-bottom: 0px;

}
</style>