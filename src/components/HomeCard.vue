<script>
export default {
  name: 'HomeCard',
  props: ['nombre', 'img']
}
</script>
<template>
  <RouterLink :to="{ name: 'product' }" class="col-12 col-md-4 px-4 mb-4">
    <div>
      <div class="card">
        <img :src="img" class="card-img-top" :alt="nombre" />
        <div class="card-body">
          <h5 class="card-title fw-bold">{{ nombre }}</h5>
        </div>
      </div>
    </div>
  </RouterLink>
</template>

<style scoped></style>
