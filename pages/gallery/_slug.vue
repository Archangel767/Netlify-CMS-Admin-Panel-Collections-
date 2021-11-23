<template>
  <div>
    <h1>{{ this.gallery }}</h1>
    <p>Path: {{ $route.path }}</p>
  </div>
</template>
<script>
  export default {
    async asyncData({ params }) {
      const gallery = params.gallery
      return { gallery }
    },
  }
</script>