<template>
<div>
<Navbar />
  <div class="about">
    <h1>This is an about page</h1>
    <p>Here is our about info</p> <br>
    <button class="button1" @click="changeButton" v-if="!signedin">Log In</button>
    <button class="button1" @click="changeButton" v-else>Log Out</button><br>
    <br>
  </div>
  <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
export default {
    name: "about",
  components: {
    Navbar,
    Footer
  },
  data() {
    return {
      signedin: true
    }
  },
  methods: {
    changeButton() {
      this.signedin= !this.signedin
    },
  }
}
</script>
<style>
.button1 {
  padding: 10px;
  background-color: black;
  color: white;
  font-weight: bold;
  font-size: 16px;        
}
</style>