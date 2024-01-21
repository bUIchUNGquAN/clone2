<template>
  <div class="bg-slate-800 rounded-lg shadow-lg rounded-lg w-60 h-72 gap-4">
    <div class="lg:py-3 px-3">
      <div v-for="(x, index) in list" :key="index" class="grid grid-cols gap-2">
        <div class="flex flex-cols">
          <img
            class="rounded-lg hover:shadow-lg hover:opacity-50 cursor-pointer"
            :src="x.imgUrl"
            alt=""
          />
          <UButton label="Pc cone" class="absolute top-[20%] left-[73%]"
            >UCRETRI</UButton
          >
          <UButton
            label="Pc cone"
            color="red"
            class="absolute top-[40%] left-[73%]"
            >Ps4</UButton
          >
        </div>
        <div
          class="w-12 h-14 bg-slate-800 absolute top-[20%] left-[90%] rounded-lg"
        >
          <p class="text-white font-bold leading-6 text-center">
            21 <span class="md:text-sm"> Diem</span>
          </p>
        </div>
        <div
          class="w-12 h-6 bg-slate-800 absolute top-[38%] left-[90%] rounded-lg"
        >
          <p class="text-white text-sm font-bold leading-6 text-center">
            19.00
          </p>
        </div>
        <div class="flex flex-wrap gap-4">
          <UIcon name="i-bx-bell" dynamic />
          <p class="text-white text-sm font-bold">{{ x.name }}</p>
        </div>
        <div class="flex flex-wrap gap-3">
          <div class="flex flex-wrap gap-2">
            <p class="text-gray-500 font-bols text-sm">
              Giriss Bedelo : <span class="text-white">{{ x.cois }} </span>
            </p>
            <div class="grid grid-cols-2 gap-9">
              <p class="text-gray-500 font-bols text-sm text-center">
                Toplam Odul <span class="text-white">{{ x.cois }}</span>
              </p>
              <p class="text-gray-500 font-bols text-sm text-center">
                Oyun Odul <span class="text-white">{{ x.modu }}</span>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-cols absolute left-[70%]">
      <MainBodyOnline />
    </div>
  </div>
</template>

<script setup>
const list = ref([
  {
    imgUrl:
      "https://images2.thanhnien.vn/528068263637045248/2023/11/7/fortnite-og-1699326064259616824163.jpg",
    name: "Forinite en iyiler turnersi",
    cois: "250 ga coin",
    modu: "5v5",
  },
]);
</script>
