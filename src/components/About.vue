<template>
  <div class="container about ">
    <div class="row">
      <div class="col-md-6">
        <div class="box">
          <h2>{{msg}}</h2>
        </div>
      </div>
      <div class="col-md-6">
        <div class="box2">
          <h2>{{msg2}}</h2>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
    msg2: String
  }
})
export default class About extends Vue {
  msg!: string;
  msg2!: string;
}
</script>

<style scoped lang="scss">
.about {
  padding: 4rem 0;
}
.box{
  height: 300px;
  width: auto;
  background: linear-gradient(rgba(0,0,0,.3), rgba(0,0,0,.3)), url(../assets/Mens-Apparel.png);
  background-size: cover;
  background-position: center;
  padding: 2rem;
  margin: 2rem 0;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;

  h2{
    color: #fff;
    font-size: 35px;
    

  }
}

.box2{
  height: 300px;
  width: auto;
  background: linear-gradient(rgba(0,0,0,.3), rgba(0,0,0,.3)), url(../assets/Womens-Apparel.jpg);
  background-size: cover;
  background-position: center;
  padding: 2rem;
  margin: 2rem 0;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;

  h2{
    color: #fff;
    font-size: 35px;
    

  }
}
</style>