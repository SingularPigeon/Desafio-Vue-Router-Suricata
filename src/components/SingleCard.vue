<script>
export default {
  name: 'SingleCard',
  props: ['nombre', 'descripcion', 'img', 'precio', 'cantidad']
}
</script>
<template>
  <div class="col-12 col-md-6 px-5 mb-4">
    <div class="card">
      <img :src="img" class="card-img-top" :alt="nombre" />
      <div class="card-body">
        <h5 class="card-title fw-bold">{{ nombre }}</h5>
        <p class="card-text">
          {{ descripcion }}
        </p>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item">Precio:$ {{ precio }}</li>
        <li class="list-group-item">Cantidad: {{ cantidad }}</li>
      </ul>
      <div class="card-body">
        <a href="#" class="card-link">Ver más</a>
        <a href="#" class="card-link">Comprar</a>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
