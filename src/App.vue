<script>
import { RouterView } from 'vue-router'
import NavBarComponent from '@/components/NavBarComponent.vue'
import FooterComponent from '@/components/FooterComponent.vue'
import MediosPago from '@/components/MediosPago.vue'

export default {
  name: 'HomeView',
  components: {
    NavBarComponent,
    FooterComponent,
    RouterView,
    MediosPago
  }
}
</script>

<template>
  <NavBarComponent />

  <RouterView />

  <MediosPago />
  <FooterComponent />
</template>
