<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>Welcome to Vue Component Demo</h1>
    <p>This app demonstrates how to properly add your own components inside Vue.js. This bit of text is served from the main <code>App</code> component.</p>
    <second-paragraph />
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer';
import SecondParagraph from './components/SecondParagraph';

export default {
  // Call the component here
  components: {
    Footer,
    SecondParagraph
  }  
}
</script>

<style>
* {
  box-sizing: border-box;
}
body {
  margin: 0;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: sans-serif;
  line-height: 2;
}
h1 {
  text-align: center;
  font-size: 2rem;
  line-height: 1.2;
}
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 1.5rem 1.5rem 15vh;
}
@media (min-width: 640px) {
  #app {
    width: 640px;
  }
}
@media (min-width: 1200px) {
  #app {
    width: 960px;
  }
}
@media (min-width: 1680px) {
  h1 {
    font-size: 3rem;
  }
  p {
    font-size: 1.25rem;
  }
}
</style>