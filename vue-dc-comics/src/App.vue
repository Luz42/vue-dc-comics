<template>
  <div id="app" class="d-flex justify-content-between flex-column">
    <!-- <img src="./assets/logo.png" alt="">
    <h1>APP</h1> -->
    <headerComponent/>
    <jumboComponent/>
    <mainComponent :cards="listDcComics"/>
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
import 'bootstrap/dist/css/bootstrap.css'
import listDcComics from '@/assets/data/dc-comics.json'
import jumboComponent from './components/jumboComponent.vue';


export default {
  name: 'App',
  components: {

    headerComponent,
    mainComponent,
    sectionNavComponent,
    sectionListComponent,
    footerComponent,
    jumboComponent


  },
  data(){return{
    listDcComics
  }}
}

</script>

<style lang="scss">


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
  
  // height: 100vh;
}


</style>
