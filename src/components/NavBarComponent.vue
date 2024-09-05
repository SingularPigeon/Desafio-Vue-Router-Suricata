<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <div>
        <RouterLink :to="{ name: 'home' }" class="navbar-brand"
          ><img src="../assets/img/logo.png" alt="logo"
        /></RouterLink>
      </div>
      <div>
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
              <RouterLink :to="{ name: 'home' }" class="nav-link link-light">Inicio</RouterLink>
            </li>

            <li class="nav-item dropdown">
              <RouterLink
                :to="{ name: 'product' }"
                class="nav-link dropdown-toggle link-light"
                id="navbarDropdown"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Productos</RouterLink
              >
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Colaciones</RouterLink
                  >
                </li>
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Bebidas</RouterLink
                  >
                </li>
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Dulces</RouterLink
                  >
                </li>
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Empanadas</RouterLink
                  >
                </li>
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Desayunos</RouterLink
                  >
                </li>
                <li>
                  <RouterLink
                    :to="{ name: 'product' }"
                    class="nav-link link-secondary dropdown-item"
                    >Verduras</RouterLink
                  >
                </li>
              </ul>
            </li>
            <li class="nav-item">
              <RouterLink :to="{ name: 'contact' }" class="nav-link link-light"
                >Contacto</RouterLink
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {}
</script>
<style scoped></style>
