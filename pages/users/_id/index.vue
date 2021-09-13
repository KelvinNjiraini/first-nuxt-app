<template>
  <h2>Single user with Id {{ $route.params.id }}</h2>
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  },
  layout: 'users',
}
</script>
