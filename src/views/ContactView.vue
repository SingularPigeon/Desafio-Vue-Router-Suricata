<script>
import ContactForm from '@/components/ContactForm.vue'
export default {
  methods: {
    volverAlHome() {
      this.$router.push({ name: 'inicio' })
    }
  },
  components: { ContactForm }
}
</script>

<template>
  <h1>Contáctanos</h1>
  <ContactForm />
  <button @click="volverAlHome"></button>
</template>
