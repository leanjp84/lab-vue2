<template>
   <div id="app">
    <Navbar />
    <h1>Welcome to the page</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. <br>Repellendus repellat dicta odit facere nam ad, suscipit adipisci. <br>Consequuntur, est recusandae vero aliquam dolores consequatur laboriosam sed, laudantium repudiandae perferendis explicabo.</p>
  <Footer />
    <router-view/>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
export default {
    name: "home",
  components: {
    Navbar,
  Footer
  }
}
</script>

<style>
</style>