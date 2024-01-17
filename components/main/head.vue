<template>
  <div
    class="lg:px-16 items-center justify-between flex text-left shadow-lg h-[80px]"
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
            variant="outline"
            placeholder="search.."
            trailing
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
              <p class="font-bold text-white gap-1 text-sm">600kVND</p>
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
            <UDropdown :items="items" :popper="{ placement: 'bottom-start' }">
                <UButton color="none" label="Quan" trailing-icon="i-heroicons-chevron-down-20-solid" />
              </UDropdown>
            <!-- <p
              class="absolute top-[25%] left-[70%] text-white font-bold text-xl flex"
            >
           
              <UIcon name="i-bx-chevron-down" dynamic class="top-[10%]" />
            </p> -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const items = [
  [{
    label: 'Profile',
    avatar: {
      src: 'https://avatars.githubusercontent.com/u/739984?v=4'
    }
  }], [{
    label: 'Edit',
    icon: 'i-heroicons-pencil-square-20-solid',
    shortcuts: ['E'],
    click: () => {
      console.log('Edit')
    }
  }, {
    label: 'Duplicate',
    icon: 'i-heroicons-document-duplicate-20-solid',
    shortcuts: ['D'],
    disabled: true
  }], [{
    label: 'Archive',
    icon: 'i-heroicons-archive-box-20-solid'
  }, {
    label: 'Move',
    icon: 'i-heroicons-arrow-right-circle-20-solid'
  }], [{
    label: 'Delete',
    icon: 'i-heroicons-trash-20-solid',
    shortcuts: ['⌘', 'D']
  }]
]
</script>