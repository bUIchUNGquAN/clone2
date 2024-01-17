<template>
  <div class="relative">
    <img src="/assets/img/body.jpg" class="opacity-50 "/>
    <div class="lg:grid grid-rows-4 gap-4 flex flex-wrap ">
      <div class="absolute top-[25%] left-[10%] grid grid-rows-1 gap-3">

        <img src="https://cdn.pixabay.com/photo/2021/08/28/09/27/pubg-mobile-logo-6580513_640.png" class="w-24 h-12 " alt="">
        <p class="text-white font-bold sm:text-3xl ">Haftalik <span class="uppercase"> pubg</span> Turnuvasi~!</p>
        <p class="text-white leading-6 font-bold sm:text-xl">Haftalik <span class="uppercase"> pubg</span> turnuvasinda buyuk oduller kazanmaya basla!</p>
        <p class="text-white leading-6 font-bold sm:text-xl">Hemen lige katil ve gelismelerden haber dar ol.</p>
        <div class=" flex flex-cols">
          <UButton label="Turnuvaya" color="red" size="xl">Turnuvaya Katil</UButton>
          <UButton label="Turnuvaya" color="" variant="ghost" class="text-white" size="xl">Detayli Bilgi </UButton>
        </div>
      </div>
      <div class="lg:py-2 grid grid-rows-1 gap-5 absolute top-[70%] left-[10%]">
        <p class="font-bold text-white xm:text-2xl">Populer Turnmuvalar</p>
        <div class="sm:flex flex-wrap items-center justify-between gap-5 ">

          <MainBodyItems v-for="x in list" ></MainBodyItems>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
  const list= ref('1,2')
</script>