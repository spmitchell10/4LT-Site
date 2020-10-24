<template>
  <div class="home">
    <!--<img alt="Vue logo" src="../assets/main_IMG.jpeg">-->
    <HelloWorld msg="For the Love of the Trail"/>

    <About 
        msg="Men's Gear"
        msg2="Women's Gear"
    />
    <FeaturedArticles/>
    <Articles
        msg="Top 10 Bike Trails in Texas"
        text1="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        msg2="Overlanding On a Budget"
        text2="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        msg3="Biking with Kid? A Beginners Guide"
        text3="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import About from '@/components/About.vue';
import Articles from '@/components/Articles.vue';
import FeaturedArticles from '@/components/FeaturedArticles.vue';
@Options({
  components: {
    HelloWorld,
    About,
    Articles,
    FeaturedArticles
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss">

.hello{
  background: linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url(../assets/main_IMG.jpg);
  height: 80vh;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
