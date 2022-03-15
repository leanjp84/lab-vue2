<template>
    <div>
    <Navbar />
  <HelloWorld />
  <Footer />
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
export default {
name: "news",
  components: {
    Navbar,
  HelloWorld,
  Footer
  }
}
</script>

<style>
</style>