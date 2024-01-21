<template>
  <div class="rounded-lg bg-slate-700 h-[150px] relative">
    <UButton class="absolute left-[44%] top-[-6%]">
      <UIcon name="i-material-symbols:swords-outline" dynamic></UIcon>
    </UButton>

    <div class="lg:grid grid-cols-3 py-12 px-10 relative">
      <!-- User 1 -->
      <div class="lg:grid grid-cols-1 gap-4 items-center">
        <img
          src="@/assets/img/avata.jpg"
          class="w-12 h-12 rounded-full"
          alt=""
        />
        <p class="text-sm font-bold text-white">Chapas</p>
      </div>

      <div class="lg:grid grid-rows-1 gap-4 items-center">
        <UIcon name="i-material-symbols:swords-outline" dynamic color="white" />
        <p class="text-sm font-bold text-white">1<span>vs</span>1</p>
      </div>

      <!-- User 2 -->
      <div class="lg:grid grid-cols-1 gap-4 items-center">
        <img
          src="@/assets/img/avata.jpg"
          class="w-12 h-12 rounded-full"
          alt=""
        />
        <p class="text-sm font-bold text-white">Chapas</p>
      </div>
    </div>
  </div>
</template>
