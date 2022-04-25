<template>
    <h1>Parfums</h1>
    <div class=" flex flex-wrap justify-around pt-4 pb-90">
        <Article v-for="(product,index) in products" :key="index" :image="product.image" :description="product.description" :price="product.price"/>
    </div>
</template>

<script>
import axios from 'axios'
import Article from '@/components/Article.vue'

export default{
  name: 'products',
  components: {
      Article,
      },
  data () {
  return {
      products: [],
    }  
  },
  created () {
    axios
      .get('./product.json')
      .then(response => (this.products = response.data.products))
  },
}
</script>
