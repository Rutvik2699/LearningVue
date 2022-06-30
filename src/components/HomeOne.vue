<template>
  <div>
    <h1>
        Home Component
    </h1>
    <my-users></my-users>
    <product-si></product-si>
  </div>
</template>

<script>

import MyUsers, {} from './MyUsers.vue'
import ProductSi from './ProductSi.vue'
export default {
    name:'HomeOne',
    components:{
      MyUsers,
      ProductSi
    }
}
</script>

<style>
  div{
    background-color: #dde5ec;
    height:500px;
    width: 100%;
  }
</style>