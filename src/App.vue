<template>
  <div id="app">
    
    <!-- Header -->
    <Header />
    <!-- Main -->
    <Main />
    <!-- Footer -->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style>

/* General */
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container{
  max-width: 1200px;
  margin: 0 auto;
}

li a{
  text-decoration: none;
  color: #000;
  transition: color 0.2s;
}

</style>
