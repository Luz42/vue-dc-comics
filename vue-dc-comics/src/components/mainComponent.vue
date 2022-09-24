<template>
    <main class="p-5">
        <h1 v-for="card in cards" :key="card.thumb" class="m-0">{{card.series}}</h1>
    </main>
  </template>
  
  <script>
  export default {
    name: 'mainComponent',
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