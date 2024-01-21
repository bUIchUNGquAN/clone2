<template>
  <header
    class="lg:px-8 items-center justify-between flex text-left shadow-lg h-[67px]"
  >
    <div class="flex items-center">
      <p class="uppercase font-bold text-2xl text-white ab">
        Gamer
        <span class="uppercase font-bold text-2xl text-red-900"> arena</span>
      </p>
    </div>
    <div class="flex gap-4 items-center float-right">
      <UInput
        type="text"
        size="xl"
        variant="outline"
        placeholder="search.."
        trailing
        color="red"
        icon="i-heroicons-magnifying-glass-20-solid"
      ></UInput>
      <UButton label="Duello Olushe" color="red"></UButton>
    </div>
    <div class="flex gap-12 items-center float-right">
      <div class="flex gap-4 items-center">
        <p class="font-bold text-white text-sm">600k VND</p>
        <UIcon name="i-bxs-circle" dynamic color="yellow" />
        <UIcon name="i-bx-credit-card" dynamic color="white" />
        <UIcon name="i-bxs-comment-dots" dynamic color="white" />
        <UIcon name="i-bx-bell" dynamic color="white" />
        <UAvatar
          chip-color="primary"
          src="https://bizweb.dktcdn.net/100/438/408/files/anh-dep-3d-yodyvn.jpg?v=1683534873601"
          size="md"
        />
        <UDropdown :items="items" :popper="{ placement: 'bottom-start' }">
          <UButton
            color="none"
            label="Quan"
            trailing-icon="i-heroicons-chevron-down-20-solid"
          />
        </UDropdown>
      </div>
    </div>
  </header>
</template>

<script setup>
const items = [
  [
    {
      label: "Profile",
      avatar: {
        src: "https://avatars.githubusercontent.com/u/739984?v=4",
      },
    },
  ],
  [
    {
      label: "Edit",
      icon: "i-heroicons-pencil-square-20-solid",
      shortcuts: ["E"],
      click: () => {
        console.log("Edit");
      },
    },
    {
      label: "Duplicate",
      icon: "i-heroicons-document-duplicate-20-solid",
      shortcuts: ["D"],
      disabled: true,
    },
  ],
  [
    {
      label: "Archive",
      icon: "i-heroicons-archive-box-20-solid",
    },
    {
      label: "Move",
      icon: "i-heroicons-arrow-right-circle-20-solid",
    },
  ],
  [
    {
      label: "Delete",
      icon: "i-heroicons-trash-20-solid",
      shortcuts: ["⌘", "D"],
    },
  ],
];
</script>
