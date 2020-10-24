<template>
  <div class="container featured-articles">
    <div class="row">
       <div class="col-md-12">
           <h2>Lorem Ipsum et Amore</h2>
           <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</h3>
       </div>
  </div>
  </div>
</template>

<script lang="ts">

import { Vue } from 'vue-class-component';
export default class FeaturedArticles extends Vue {

}
</script>

<style scoped lang="scss">

.featured-articles{
  text-align: center;
  padding: 4rem 0;
  h2{
    font-size: 70px;
    font-weight: bold;
  }
  h3{
    font-size: 30px;
    max-width: 60%;
    margin: 0 auto;
  }
}

</style>