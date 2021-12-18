<template>
  <h1>Welcome to Products</h1>
  <div class="container-fluid">
    <product-list :product="this.product"></product-list>
  </div>
  <product-create-form @created="addProduct"></product-create-form>
</template>

<script>
export default {
  methods: {
    addProduct (productLocation) {
      const endpoint = process.env.VUE_APP_BACKEND_BASE_URL + productLocation
      const requestOptions = {
        method: 'GET',
        redirect: 'follow'
      }
      fetch(endpoint, requestOptions)
        .then(response => response.json())
        .then(product => this.product.push(product))
        .catch(error => console.log('error', error))
    }
  },
  mounted () {
    const requestOptions = {
      method: 'GET',
      redirect: 'follow'
    }
    fetch('http://localhost:8080/web/product', requestOptions)
      .then(response => response.json())
      .then(result => console.log(result))
      .catch(error => console.log('error', error))
  }
}
</script>

<style scoped>
</style>
