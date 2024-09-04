<script>
import HomeCard from '@/components/HomeCard.vue'
import productData from '@/productos-data.json'
export default {
  name: 'ProductView',
  components: {
    HomeCard
  },
  props: {
    nombre: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      products: productData.products
    }
  }
}
</script>

<template>
  <section class="container" id="productos">
    <h1 class="text-center">Nuestros Productos</h1>
    <div class="row">
      <HomeCard
        v-for="product in products"
        :key="product.id"
        :nombre="product.nombre"
        :img="product.img"
      />
    </div>
  </section>
</template>
