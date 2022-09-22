<template>
    <header class="d-flex justify-content-between p-2">
        <picture>
            <img class="img-fluid" src="../assets/img/dc-logo.png" alt="">
        </picture>
        <headerNavComponent/>
    </header>
  </template>
  
  <script>
    import headerNavComponent from './headerNavComponent.vue';
  
    export default {
    name: 'headerComponent',
    components:{
        headerNavComponent
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    

    header{
        background-color: #ffffff;
        display: flex;
        justify-content: space-between;
        img{
            width: 50px;
        }
    }
  
  </style>
  