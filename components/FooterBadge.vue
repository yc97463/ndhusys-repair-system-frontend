<template>
  <div class="my-3 mr-5">
    <span class="px-4 py-1 text-sm bg-white rounded-full">{{ title }}</span>
    <span class="ml-2">{{ content }}</span>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    content: {
      type: String,
      required: true
    }
  }
}
</script>