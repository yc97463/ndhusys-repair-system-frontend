<template>
  <NuxtLink :to=url>
    <div class="w-full my-4 px-6 py-4 rounded-lg shadow-md shadow-black/40 hover:shadow-black/60">
      <div class="grid grid-cols-6 gap-4 content-center">
        <div class="col-start-1 col-span-1 col-end-1 grid content-center">
          <div class="w-12 h-12 bg-gray-400/[.25] rounded-full flex justify-center items-center">
            <img :src="`/assets/icon/${icon}_.svg`" class="w-auto h-6" />
          </div>
        </div>
        <div class="col-start-2 col-span-6">
          <h1 class="text-xl font-semibold">{{ title }}</h1>
          <p class="text-sm text-gray-500">{{ description }}</p>
        </div>
        <div class="col-end-11 col-span-2 grid content-center">
          <div
            class="px-4 py-2 bg-white text-center border border-black rounded-md shadow-sm hover:shadow-sm hover:shadow-black/80">
            {{
              action == "apply" ? "申請" : "前往" }}
            <!-- an right arrow svg icon -->
            <svg class="w-4 h-4 inline-block" viewBox="0 0 7 12" fill="none">
              <path d="M1 1L6 6L1 11" stroke="black" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </NuxtLink>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    },
    action: {
      type: String,
      required: true
    },
    url: {
      type: String,
      required: false
    }
  }
}
</script>