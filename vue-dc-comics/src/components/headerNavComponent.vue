<template>
    <nav class="col d-flex">
        <ul class="nav d-flex align-items-center flex-shrink-0">
            <li @click="setActiveIndex(index)" 
                v-for="(name, index) in linkNav" v-bind:key="name" 
                :class="index === activeIndex ? 'ae-active' : ''" 
                class="nav-item h-100 d-flex align-items-center text-uppercase fw-bold" 
                style="color: black;">
                    <a class="nav-link" style="color: inherit; font-size: 0.8em;" aria-current="page" href="#">{{ name }}</a>
            </li>  
        </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'headerNavComponent',
    data(){
       return {
        activeIndex: 0,
        linkNav: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
       }
    },
    methods:{
        setActiveIndex(index){
            this.activeIndex = index
        }
    }

  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">

    .ae-active{
        color: blue !important;
        border-bottom: 3px solid blue !important;

    }

  
  </style>
  