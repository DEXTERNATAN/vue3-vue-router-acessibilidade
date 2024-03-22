<template>
  <h1>About</h1>
  <HelloWorld mag="TEST" />
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue'
export default {
  components: { HelloWorld },
  mounted() {
    console.log('mounted About page')

    console.log(`Teste`)
    const script = document.createElement('script')
    script.src = 'https://cdn-scorea11y.estaleiro.serpro.gov.br/a11y-tracking.js'
    script.async = true
    document.head.appendChild(script)
  },
  unmounted() {
    console.log('unmounted About page')
  },
}
</script>
