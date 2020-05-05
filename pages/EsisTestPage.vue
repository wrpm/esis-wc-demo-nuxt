<template>
  <div >
    <h1>Samsung wrapper</h1>

    <div ref="container" id="container">
      <esis-app></esis-app>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EsisTestPage',
  computed: {},
  created() {
    if (process.server) return
    // let containerElement = this.$refs.container
    let containerElement = document.getElementById('container')

    let esisScript = document.createElement('script');
    esisScript.setAttribute('src',"http://esis.wearepm.co/app.10af994f.js");

    // let esisStyles = document.createElement('link')
    // esisStyles.setAttribute('href', 'http://esis.wearepm.co/app.f84c632a.css')
    // esisStyles.setAttribute('rel', 'stylesheet')
    // esisStyles.setAttribute('type', 'text/css')

    containerElement.appendChild(esisScript)
    // containerElement.appendChild(esisStyles)
    // document.head.appendChild(esisScript);
  },
}
</script>

<style scoped>
div {
  display: flex;
  width: 100%;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

h1 {
  margin-top: 2rem;
  margin-bottom: 2rem;
  color: #35495e;
}
</style>
