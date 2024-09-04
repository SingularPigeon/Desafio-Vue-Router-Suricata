<script>
import SingleCard from '@/components/SingleCard.vue'
import productData from '@/productos-data.json'
export default {
  name: 'ProductView',
  components: {
    SingleCard
  },
  props: {
    nombre: {
      type: String,
      required: true
    },
    descripcion: {
      type: String,
      required: true
    },
    precio: {
      type: Number,
      required: true
    },
    cantidad: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      products: productData.products
    }
  },
  methods: {
    volverAlHome() {
      return this.$router.push({ name: 'inicio' })
    }
  }
}
</script>

<template>
  <section class="container" id="productos">
    <h1 class="text-center">Nuestros Productos</h1>
    <div class="row">
      <!-- primera -->

      <SingleCard
        v-for="product in products"
        :key="product.id"
        :nombre="product.nombre"
        :descripcion="product.descripcion"
        :img="product.img"
        :precio="product.precio"
        :cantidad="product.cantidad"
      />
    </div>
    <button @click="volverAlHome">Volver al inicio</button>
  </section>
</template>
