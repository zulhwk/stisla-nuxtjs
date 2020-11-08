<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  head: {
    link: [
      { rel: 'stylesheet', src: require('@/assets/stisla/css/style.css') },
      { rel: 'stylesheet', src: require('@/assets/stisla/css/components.css') }
    ]
  }
}
</script>
