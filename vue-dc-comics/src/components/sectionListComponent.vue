<template>
    <section>
      <div class="container-xl">
        <div class="row">
          <div style="color:white" class="col-6">
            <div class="row py-5">
              <listComponent label="Dc Comics" :links="dcComics"/>
              <listComponent label="dc" :links="dc"/>
              <listComponent label="sites" :links="sites"/>
              <listComponent label="shop" :links="shop"/>
            </div>
          </div>
          <picture class="col-6">
            <!-- <img class="img-fluid" src="@/assets/img/dc-logo-bg.png" alt=""> -->
          </picture>
        </div>
      </div> 
    </section>
  </template>
  
  <script>
  import listComponent from './listComponent.vue';
  import { dcComics, shop, dc, sites } from '../assets/data/listListsFooter.js'

  export default {
    name: 'sectionListComponent',
    components:{
      listComponent
    },
    data(){return{
      dcComics,
      shop,
      dc,
      sites
    }}
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">

    section{
        width: 100%;
        background-image:url("../assets/img/footer-bg.jpg") ;
        background-repeat: no-repeat;
        background-size: cover;
        flex-grow: 1;
    };

    picture{
      background-image:url("../assets/img/dc-logo-bg.png") ;
      background-repeat: no-repeat;
      background-size: cover;
      background-position-y: center;
    }

  </style>