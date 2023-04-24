<template>
  <a :href="url" target=" _blank" class="text-white pl-3.5" rel="noopener noreferrer">
    {{ name }}
  </a>
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
  }
}
</script>