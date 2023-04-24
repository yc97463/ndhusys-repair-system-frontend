<template>
  <div>
    <div class="w-screen border-b-2 border-ndhu-green">
      <div class="w-screen h-7 bg-ndhu-green/[.85]">
        <div class="w-2/3 mx-auto">
          <div class="float-right">
            <HeaderTopLinks name="東華大學" url="https://www.ndhu.edu.tw/" />
            <HeaderTopLinks name="總務處" url="https://ga.ndhu.edu.tw/" />
            <HeaderTopLinks name="東華 i 溝通" url="https://web.ndhu.edu.tw/SCR/pprz/Login.aspx" />
          </div>
        </div>
      </div>
      <div class="w-screen h-16">
        <div class="w-2/3 mx-auto">
          <div class="my-8">
            <div class="float-left">
              <NuxtLink to="/" class="text-xl align-middle">
                總務處維修系統
              </NuxtLink>
            </div>
            <div class="float-right">
              <NavLinks name="維修查詢" url="/" />
              <NavLinks name="報修申請" url="/about" />
              <NavLinks name="使用說明" url="/" />
              <NuxtLink to="/auth/login" class="ml-3.5 text-white bg-ndhu-green rounded-lg px-7 py-2"
                rel="noopener noreferrer">
                登入
              </NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="w-screen">
      <slot />
    </div>
    <div
      class="w-screen bg-[url('/footer_ndhubuildings.png')] bg-neutral-200/60 bg-no-repeat bg-right-bottom bg-cover h-36 absolute inset-x-0 bottom-0">
      <div class="w-2/3 mx-auto">
        <FooterBadge title="程式版本" content="beta-20230424" />
        <FooterBadge title="所在分流" content="SYSVM 17" />
        <FooterBadge title="業務單位" content="總務處 (03) 890 6370" />
      </div>
    </div>
  </div>
</template>