<template>
  <div id="app">
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png" />
    <nav><router-link to="/">Home</router-link> | <router-link to="/about">About</router-link></nav>
    <main>
      <router-view />
    </main>
  </div>
</template>

<script>
export default {
  created() {
    console.log(`Teste`)
    const script = document.createElement('script')
    script.src = 'https://cdn-scorea11y.estaleiro.serpro.gov.br/a11y-tracking.js'
    script.async = true
    document.head.appendChild(script)
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
