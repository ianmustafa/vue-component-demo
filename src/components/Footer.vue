<template>
  <p>Copyright &copy; {{ year }} <a href="https://github.com/ianmustafa" target="_blank">Ian Mustafa</a>. Find the repo of this project <a href="https://github.com/ianmustafa/vue-component-demo" target="_blank">here</a>.</p>
</template>

<script>
export default {
  name: 'Footer',
  data: () => ({
    year: (new Date).getFullYear()
  })
}
</script>

<style scoped>
p {
  margin-top: 2rem;
  font-size: 0.75rem;
  color: #676767;
}
a {
  text-decoration: none;
  color: #424242;
}
a:hover, a:focus, a:active {
  text-decoration: underline;
}
@media (min-width: 1680px) {
  p {
    font-size: 1rem;
  }
}
</style>