<template>
  <div>
    <h1>Nuestros Productos</h1>
    <ul>
      <li v-for="product in products" :key="product.id">
        <router-link :to="{ name: 'ProductCategory', params: { id: product.id } }">{{
          product.nombre
        }}</router-link>
      </li>
    </ul>
    <!-- Aquí se cargará el detalle del producto seleccionado -->
    <router-view></router-view>
  </div>
</template>

<script>
import productsData from '@/productos.json'

export default {
  data() {
    return {
      products: productsData.products
    }
  }
}
</script>
