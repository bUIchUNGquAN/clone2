<template>
  <div class="rounded-lg bg-slate-700 h-[150px] relative">
    <UButton class="absolute left-[44%] top-[-6%]">
      <UIcon name="i-bx-knife" dynamic></UIcon>
    </UButton>

    <div class="lg:flex flex-rows py-12 px-10 relative">
      <!-- User 1 -->
      <div class="lg:grid grid-cols-1 gap-4 items-center">
        <img
          src="@/assets/img/avata.jpg"
          class="w-12 h-12 rounded-full"
          alt=""
        />
        <p class="text-sm font-bold text-white">Chapas</p>
      </div>

      <!-- Knives -->
      <div class="flex items-center scale-150">
        <UIcon name="i-bx-knife" dynamic color="white" class="rotate-180" />
        <UIcon name="i-bx-knife" dynamic color="white" class="rotate-90" />
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
