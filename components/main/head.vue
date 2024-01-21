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
        color="white"
        icon="i-heroicons-magnifying-glass-20-solid"
        @input="handleSearch"
      ></UInput>
      <UButton
        label="Duello Olushe"
        color="red"
        :loading="loading"
        @click="handleDuelloClick"
      ></UButton>
    </div>
    <div class="flex gap-12 items-center float-right">
      <div class="flex gap-4 items-center">
        <UIcon
          name="i-bx-credit-card"
          dynamic
          color="white"
          @click="showNotification"
        />
        <div v-if="notificationVisible" class="notification">
          <!-- Your notification content goes here -->
          <p class="font-bold text-white text-sm">
            nap thanh cong 600k VND
            <UIcon name="i-bxs-circle" dynamic color="yellow" />
          </p>
        </div>
        <UIcon name="i-bxs-comment-dots" dynamic color="white" />
        <UIcon name="i-bx-bell" dynamic color="white" />
        <UAvatar
          chip-color="primary"
          src="https://bizweb.dktcdn.net/100/438/408/files/anh-dep-3d-yodyvn.jpg?v=1683534873601"
          size="md"
        />
        <UDropdown
          :items="items"
          mode="hover"
          :popper="{ placement: 'bottom-start' }"
        >
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
// dropdow
const items = [
  [
    {
      label: "buichungquan@gmail.com",
      slot: "account",
      disabled: true,
    },
  ],
  [
    {
      label: "Settings",
      icon: "i-heroicons-cog-8-tooth",
    },
  ],
  [
    {
      label: "Documentation",
      icon: "i-heroicons-book-open",
    },
    {
      label: "Changelog",
      icon: "i-heroicons-megaphone",
    },
    {
      label: "Status",
      icon: "i-heroicons-signal",
    },
  ],
  [
    {
      label: "Sign out",
      icon: "i-heroicons-arrow-left-on-rectangle",
    },
  ],
];
// loading search
const loading = ref(false);
const handleSearch = () => {
  loading.value = true;

  setTimeout(() => {
    loading.value = false;
  }, 2000);
};

// show thong bao
const notificationVisible = ref(false);
const showNotification = () => {
  notificationVisible.value = true;
  setTimeout(() => {
    notificationVisible.value = false;
  }, 3000);
};
</script>
