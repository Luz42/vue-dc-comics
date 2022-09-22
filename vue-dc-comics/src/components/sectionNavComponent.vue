<template>
    <section class="p-5">
      <div class="row">
        <div v-for="element in elementSection" v-bind:key="element" class="col p-2 d-flex align-items-center">
          <img class="img-fluid h-50" :src="`../assets/img/buy-${element}`" :alt="element">
          <h6 class="text-uppercase flex-shrink-0 m-0 mx-2" style="color: white;">{{element}}</h6>
        </div>
      </div>  
      </section>
  </template>
  
  <script>
  export default {
    name: 'sectionNavComponent',
    data(){
      return{
      elementSection:['comics-digital-comics.png', 'comics-merchandise.png', 'comics-shop-locator.png', 'comics-subscriptions.png', 'dc-power-visa.svg']
      }
  }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    

    section{
        width: 100%;
        background-color: #0282f9;
    }

  </style>