<template>
  <div style="font-size:0.8em">
    <h4 class="text-uppercase" style="font-weight:bold">{{ label }}</h4>
    <ul class="p-0">
        <li class="text-capitalize" v-for="link in links" :key="link">
        <a href="#">
            {{ link }}
        </a>
        </li>
    </ul>
  </div>
</template>

<script>
export default {

    name: 'listComponent',
    props:{
        links: Array,
        label: String
    }

}
</script>

<style scoped lang="scss">

li{
    list-style-type: none;
    a{
        color: grey;
        text-decoration: none;
    }
}

</style>