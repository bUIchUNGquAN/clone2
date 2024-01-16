<template>
  <div
    class="lg:px-16 items-center justify-between flex text-left shadow-lg h-[70px]"
  >
    <div class="flex flex-cols-4 items-center justify-between relative w-full">
      <div class="flex flex-shrink-0 items-center">
        <p class="uppercase font-bold text-3xl text-white ab">
          Gamer
          <span class="uppercase font-bold text-3xl text-red-900"> arena</span>
        </p>
        <div class="lg:flex flex-cols gap-4 absolute left-[25%]">
          <UInput
            type="text"
            size="xl"
            variant="ghost"
            placeholder="search.."
            trailing="false"
            color="red"
            icon="i-heroicons-magnifying-glass-20-solid"
          >
          </UInput>
          <UButton label="Duello Olushe" color="red"></UButton>
        </div>
        <div class="lg:grid grid-cols-4 gap-0 h-24 py-8 px-8 absolute right-0">
          <div class="sm:grid grid-cols-2 gap-1 absolute top-[30%]">
            <div
              class="sm:flex flex-cols gap-1 absolute right-[480%] top-[30%]"
            >
              <p class="font-bold text-white gap-1 text-sm">600k VND</p>
              <UIcon
                name="i-bxs-circle"
                dynamic
                color="yellow"
                class="absolute left-[110%] top-[20%]"
              />
            </div>
            <UIcon
              name="i-bx-credit-card"
              dynamic
              size="sm"
              color="white"
              class="absolute right-[300%] top-[8%]"
            />
            <UIcon
              name="i-bxs-comment-dots"
              dynamic
              size="sm"
              color="white"
              class="absolute right-[200%] top-[8%]"
            />

            <UIcon
              name="i-bx-bell"
              dynamic
              size="sm"
              color="white"
              class="absolute right-[110%]"
            />

            <UAvatar
              chip-color="primary"
              src="https://bizweb.dktcdn.net/100/438/408/files/anh-dep-3d-yodyvn.jpg?v=1683534873601"
              size="md"
            />
            <p
              class="absolute top-[25%] left-[70%] text-white font-bold text-xl flex"
            >
              Quan
              <UIcon name="i-bx-chevron-down" dynamic class="top-[10%]" />
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
