<template>
  <div class="container articles">
    <div class="row">
      <div class="col-md-2 article-title">
        <h2>Featured</h2>
      </div>
      <div class="col-md-5 article-card">
        <div class="article-wrap">
          <div class="article-box">
            <h2>{{msg}}</h2>
          </div>
          <!-- <div class="article-exerpt">
            <p>{{text1}}</p>
          </div>-->
        </div>
      </div>
      <div class="col-md-5 article-card">
        <div class="article-box2">
          <h2>{{msg2}}</h2>
        </div>
        <!-- <div class="article-exerpt">
          <p>{{text2}}</p>
        </div>-->
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
    msg2: String,
    msg3: String,
    text1: String,
    text2: String,
    text3: String
  }
})
export default class Artibles extends Vue {
  msg!: string;
  msg2!: string;
  msg3!: string;
  text1!: string;
  text2!: string;
  text3!: string;
}
</script>

<style scoped lang="scss">
.articles {
  padding-top: 5rem;
  padding-bottom: 5rem;

.article-title{
    h2{
        font-size: 35px;
    }
}
  .article-card {

    .article-box {
      height: 250px;
      width: auto;
      background: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
        url(../assets/stock_IMG-1.jpg);
      background-size: cover;
      background-position: center;
      padding: 2rem;
      border-radius: 10px;
      display: flex;
      justify-content: center;
      align-items: center;

      h2 {
        color: #fff;
        font-size: 25px;
        text-align: center;
      }
      p {
        margin: 0;
        font-size: 18px;
      }
    }

    .article-box2 {
      height: 250px;
      width: auto;
      background: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
        url(../assets/stock_IMG-2.png);
      background-size: cover;
      background-position: center;
      padding: 2rem;
      border-radius: 10px;
      display: flex;
      justify-content: center;
      align-items: center;

      h2 {
        color: #fff;
        font-size: 25px;
        text-align: center;
      }
    }
    .article-exerpt {
      p {
        margin: 0;
        padding: 0.5rem 1rem;
        font-size: 16px;
      }
    }
  }
}
</style>