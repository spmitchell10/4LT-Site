<template>
  <div id="nav">
    <router-link to="/">Gear</router-link>
    <router-link to="/about">Stories</router-link>
    <router-link to="/portfolio">Trails</router-link>
    <router-link to="/experience">Photography</router-link>
  </div>
  <router-view/>
</template>

<style lang="scss">

@import "./sass/_resets.scss";
@import "./sass/_base.scss";


</style>
