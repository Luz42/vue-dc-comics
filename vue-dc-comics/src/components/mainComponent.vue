<template>
    <main>
      <div class="container-fluid p-5"> 
        <div class="row">
          <cardMainComponents :cardData="card" v-for="card in cards" :key="card.series"/>
          <!-- <div v-for="card in cards" :key="card.series"  class="col-2">{{ card.thumb }}</div> -->
        </div>
          <!-- <img :src="card.thumb" alt=""> -->
      </div>
    </main>
  </template>
  
  <script>
  import cardMainComponents from '@/components/cardMainComponent.vue'

  export default {
    name: 'mainComponent',
    components:{
     cardMainComponents
    },

    props: {
      cards: Array
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">

    main{
        background-color:  #1c1c1c;
        color: white;
    }

  </style>