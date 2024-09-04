<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <RouterLink :to="{ name: 'home' }" class="nav-link">Inicio</RouterLink>
          </li>

          <li class="nav-item dropdown">
            <RouterLink
              :to="{ name: 'product' }"
              class="nav-link dropdown-toggle"
              id="navbarDropdown"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              Productos</RouterLink
            >
            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Colaciones</RouterLink
                >
              </li>
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Bebidas</RouterLink
                >
              </li>
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Dulces</RouterLink
                >
              </li>
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Empanadas</RouterLink
                >
              </li>
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Desayunos</RouterLink
                >
              </li>
              <li>
                <RouterLink :to="{ name: 'product' }" class="nav-link dropdown-item"
                  >Verduras</RouterLink
                >
              </li>
            </ul>
          </li>
          <li class="nav-item">
            <RouterLink :to="{ name: 'contact' }" class="nav-link">Contacto</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script>
export default {}
</script>
<style scoped></style>
