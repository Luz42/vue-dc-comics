<template>
    <section>
      <div class="container-fluid">
        <div class="row">
          <div style="color:white" class="col-6 d-flex flex-wrap">
            <listComponent label="Dc" :links="dcLinks"/>
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

  export default {
    name: 'sectionListComponent',
    components:{
      listComponent
    },
    data(){return{
      dcLinks: ['batman', 'superman','wonderWoman','flash']
    }}
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">

    section{
        width: 100%;
        padding: 50px;
        background-image:url("../assets/img/footer-bg.jpg") ;
        background-repeat: no-repeat;
        background-size: cover;
        flex-grow: 1;
    };

    picture{
      background-image:url("../assets/img/dc-logo-bg.png") ;
      background-repeat: no-repeat;
      background-size: cover;
    }

  </style>