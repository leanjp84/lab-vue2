<template>
<div>
  <Navbar />
  <div class="about">
      <h1>Contact Us</h1>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed, qui iste asperiores enim nostrum molestiae <br>adipisci laborum aspernatur maiores aliquam praesentium eveniet culpa maxime nemo! <br>Deleniti soluta ipsum expedita consequatur!</p>
       </div>
  <Footer />
</div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'ContactUs',
  components: {
    Navbar,
    Footer
  }
}
</script>