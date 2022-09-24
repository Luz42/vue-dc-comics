<template>
    <section>
      <div class="container-xl">
        <div class="row d-flex flex-nowrap">
          <div v-for="element in elementSection" v-bind:key="element" class="col px-2 d-flex align-items-center">
            <img class="img-fluid h-25" :src="`./img/buy-${element}`" :alt="element">
            <h6 class="text-uppercase m-0 px-2" style="color: white; font-size: 0.7em;">{{element}}</h6>
          </div>
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