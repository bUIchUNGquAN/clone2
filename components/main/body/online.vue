<template>
  <div class="flex flex-cols gap-9">
    <UAvatarGroup size="xs" :max="4">
      <UAvatar v-for="(avata, index) in avata" :key="index" :src="avata.src" />
    </UAvatarGroup>
    <div class="flex flex-wrap">
      <p class="text-white text-sm cursor-pointer" @click="addAvata">
        {{ `${avata.length} /25` }} Online
      </p>
      <UButton @click="removeAvatar" variant="ghost" />
    </div>
  </div>
</template>

<script setup>
const avata = ref([
  {
    src: "https://anhgaisexy.com/wp-content/uploads/2022/01/20210910-hoang-ngoc-linh-9.jpg",
  },
]);
const addAvata = () => {
  if (avata.value.length < 25) {
    avata.value.push(
      "https://anhgaisexy.com/wp-content/uploads/2022/01/20210910-hoang-ngoc-linh-9.jpg"
    );
  }
};
const removeAvatar = () => {
  if (avata.value.length > 0) {
    avata.value.pop();
  }
};
</script>
