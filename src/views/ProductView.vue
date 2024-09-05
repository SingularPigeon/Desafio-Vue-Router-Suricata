/** Mi idea era que de cada card del home se accedieria a la categoría de productos con sus card
(bebidas, desayunos,etc), pero no pude resolverlo 🫡 */

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
      return this.$router.push({ name: 'home' })
    }
  }
}
</script>

<template>
  <section class="container text-center" id="productos">
    <h1 class="text-center">Nuestros Productos</h1>
    <button class="btn btn-secondary border-0 text-light bg-suricata mb-5" @click="volverAlHome">
      Volver al inicio
    </button>

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
  </section>
</template>
