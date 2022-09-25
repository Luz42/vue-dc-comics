<template>
  <div class="col-2 p-2">
    <img class="img-fluid" :src="cardData.thumb" alt="">
  </div>
</template>

<script>

export default {

    name: 'cardMainComponent',
    props:{
        cardData: Object
    }

}
</script>

<style>

</style>