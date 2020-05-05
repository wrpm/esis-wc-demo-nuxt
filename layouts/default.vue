<template>
  <div>
    <nav>
      <nuxt-link class="link" :to="'/'">Home</nuxt-link>
      <nuxt-link class="link" :to="'/catalogue'">Catalogue</nuxt-link>
      <nuxt-link class="link" :to="'/esis-test-page'">Smasung</nuxt-link>
    </nav>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

nav {
  width: 100%;
  display: flex;
  justify-content: center;
}
.link {
  text-decoration: none;
  color: #35495e;
  font-size: 1.5;
  margin-right: 2rem;
  padding: 1rem;
}

.link:hover {
  color: #3b8070;
}
</style>
