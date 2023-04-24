<template>
  <NuxtLink :to=url>
    <div class="w-full my-4 px-6 py-4 rounded-lg border-2 hover:border-black/60">
      <div class="grid grid-cols-6 gap-4 content-center">
        <div class="col-start-1 col-span-1 col-end-1 grid content-center">
          <div class="w-12 h-12 bg-gray-400/[.25] rounded-full flex justify-center items-center">
            <img :src="`/assets/icon/${icon}_.svg`" class="w-auto h-6" />
          </div>
        </div>
        <div class="col-start-2 col-span-6">
          <h1 class="text-xl font-normal">{{ title }}</h1>
          <p class="text-sm text-gray-500">{{ description }}</p>
        </div>
        <div class="col-end-11 col-span-2 grid content-center">
          <div class="px-4 py-2 bg-white text-center border border-black rounded-md">
            {{
              action == "apply" ? "申請" : "前往" }}
            <svg class="w-3 h-3 inline-block align-baseline" viewBox="0 0 12 12" fill="none"
              xmlns="http://www.w3.org/2000/svg">
              <path d="M11 1H7.66667M11 1L6 6M11 1V4.33333" stroke="black" stroke-width="1.2" stroke-linecap="round"
                stroke-linejoin="round" />
              <path
                d="M11 6.55556V9.88889C11 10.5026 10.5026 11 9.88889 11H2.11111C1.49746 11 1 10.5026 1 9.88889V2.11111C1 1.49746 1.49746 1 2.11111 1H5.44444"
                stroke="black" stroke-width="1.2" stroke-linecap="round" />
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