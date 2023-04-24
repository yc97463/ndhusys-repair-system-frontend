<template>
  <NuxtLink :to="url" class="pl-3.5" rel="noopener noreferrer">
    {{ name }}
  </NuxtLink>
</template>

<script>

export default {
  props: {
    name: {
      type: String,
      required: true
    },
    url: {
      type: String,
      required: true
    }
  },
}
</script>