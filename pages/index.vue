<template>
  <div class="w-1/3 mx-auto my-16">
    <h1 class="text-center font-semibold text-2xl">請選擇維修類別</h1>
    <div class="">
      <RepairChoosenCard icon="building" title="校舍宿舍報修" description="總務處校舍、宿舍維修相關通報。" action="apply"
        url="/auth/login?redirec=/repair" />
      <RepairChoosenCard icon="wifi-issue" title="網路異常報修" description="圖資中心宿舍網路斷線、異常報修。" action="go"
        url="http://134.208.12.37/repair/" />
      <RepairChoosenCard icon="wrench" title="教學設備報修" description="教學卓越中心教室、教學設備報修。" action="go"
        url="http://cte.ndhu.edu.tw/cen3/fix/" />
    </div>
  </div>
</template>

<script setup>
useHead({
  title: '請選擇維修類別 - 總務處維修系統',
  meta: [
    { name: 'description', content: '請選擇維修類別 - 總務處維修系統' }
  ],
})
</script>