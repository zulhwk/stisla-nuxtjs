<template>
  <a href="#">
    <b-button variant="outline-dark" class="mb-3">
      {{ name }}
    </b-button>
  </a>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: 'TAGS'
    }
  }
}
</script>
