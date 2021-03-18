<template>
  <div class="home">
    <Navbar/>
    <div class="container">
      <Hero/>

      <div class="row mt-3">
        <div class="col-md-6">
          <h2>Popular <strong>Books</strong></h2>
        </div>
        <div class="col-md-6">
          <router-link class="btn btn-md btn-warning float-right" to="/books">See All</router-link>
        </div>
      </div>

      <div class="row mt-3">
        <div class="col-md-4">
          <ProductCard/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Hero from '@/components/Hero.vue'
import ProductCard from '@/components/ProductCard.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Hero,
    ProductCard
  }
}
</script>
