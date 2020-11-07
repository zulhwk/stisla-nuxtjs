<template>
  <div class="card card-primary">
    <div class="card-header">
      <h4>{{ title }}</h4>
    </div>
    <div class="card-body">
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Title'
    }
  }
}
</script>
