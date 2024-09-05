<script>
import ContactForm from '@/components/ContactForm.vue'
export default {
  methods: {
    volverAlHome() {
      this.$router.push({ name: 'home' })
    }
  },
  components: { ContactForm }
}
</script>

<template>
  <div class="container my-5">
    <button class="btn btn-secondary border-0 text-light bg-suricata mb-5" @click="volverAlHome">
      Volver al inicio
    </button>
    <h1>Contáctanos</h1>
    <ContactForm />
  </div>
</template>
