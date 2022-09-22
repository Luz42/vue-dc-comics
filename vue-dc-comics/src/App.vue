<template>
  <div id="app">
    <!-- <img src="./assets/logo.png" alt="">
    <h1>APP</h1> -->
    <headerComponent/>
    <mainComponent/>
    <sectionNavComponent/>
    <sectionListComponent/>
    <footerComponent/>
  </div>
</template>

<script>
import headerComponent from './components/headerComponent.vue';
import mainComponent from './components/mainComponent.vue';
import sectionNavComponent from './components/sectionNavComponent.vue';
import sectionListComponent from './components/sectionListComponent.vue';
import footerComponent from './components/footerComponent.vue';

export default {
  name: 'App',
  components: {

    headerComponent,
    mainComponent,
    sectionNavComponent,
    sectionListComponent,
    footerComponent

  }
}
</script>

<style lang="scss">
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
  display: flex;
  flex-direction: column;
  height: 100vh;
}


</style>
