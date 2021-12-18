<template>
  <div class="row row-cols-1 row-cols-md-4 g-4">
    <div class="col" v-for="product in products" :key="product.id">
      <div class="card h-100">
        <img :src="getProduct(product)" class="card-img-top" :alt="product.name">
        <div class="card-body">
          <h5 class="card-title">{{ product.id }} {{ product.name }}</h5>
          <p class="card-text">
            Das Product {{ product.name }} kostet {{ product.price}}.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductList',
  props: {
    product: {
      type: Array,
      required: true
    }
  },
  methods: {
    getProduct (product) {
      if (product.name === true) {
        return require('../assets/logo.png')
        // eslint-disable-next-line import/no-webpack-loader-syntax
      } else require('Bitte Produkt auswählen!')
    }
  }
}
</script>

<style scoped>
</style>
