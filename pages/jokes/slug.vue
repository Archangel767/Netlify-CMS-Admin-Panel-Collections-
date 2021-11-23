<template>
  <div>
    <h1>{{ this.jokes }}</h1>
    <p>Path: {{ $route.path }}</p>
  </div>
</template>
<script>
  export default {
    async asyncData({ params }) {
      const jokes = params.jokes
      return { jokes }
    },
  }
</script>