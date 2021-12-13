<template>
  <div class="home">
    <img alt="Blue Shield logo" src="../assets/BlueShield.png">
    <HelloWorld msg="Welcome to Indizon"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
