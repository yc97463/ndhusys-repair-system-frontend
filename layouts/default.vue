<template>
  <div class="min-h-screen">
    <div class="w-screen border-b-2 border-ndhu-green">
      <div class="w-screen h-10 bg-ndhu-green/[.85]">
        <div class="w-10/12 mx-auto py-2 md:w-2/3">
          <div class="float-right text-sm">
            <HeaderTopLinks name="東華大學" url="https://www.ndhu.edu.tw/" />
            <HeaderTopLinks name="總務處" url="https://ga.ndhu.edu.tw/" />
            <HeaderTopLinks name="東華 i 溝通" url="https://web.ndhu.edu.tw/SCR/pprz/Login.aspx" />
          </div>
        </div>
      </div>
      <div class="w-screen h-16">
        <div class="w-10/12 mx-auto md:w-2/3">
          <div class="my-8 grid grid-cols-2 gap-4">
            <div class="col-start-1 col-span-1">
              <NuxtLink to="/" class="text-xl align-middle self-center">
                總務處維修系統
              </NuxtLink>
            </div>
            <div class="col-end-3 col-span-1">
              <div class="float-right">
                <!-- <NavLinks name="維修查詢" url="/" />
              <NavLinks name="報修申請" url="/about" />
              <NavLinks name="使用說明" url="/" /> -->
                <NuxtLink to="/auth/login" class="ml-3.5 text-white bg-ndhu-green rounded-lg px-7 py-2"
                  rel="noopener noreferrer">
                  登入
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="w-screen">
      <slot />
    </div>
    <div
      class="w-screen bg-[url('/footer_ndhubuildings.png')] bg-neutral-200/60 bg-no-repeat bg-right-bottom bg-cover h-36 flex">
      <div class="w-10/12 mx-auto self-center md:w-2/3">
        <FooterBadge title="程式版本" content="beta-20230424" />
        <FooterBadge title="所在分流" content="SYSVM 17" />
        <FooterBadge title="業務單位" content="總務處 (03) 890 6370" />
      </div>
    </div>
  </div>
</template>