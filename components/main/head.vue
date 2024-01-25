<template>
  <header
    class="px-8 items-center justify-between flex text-left shadow-lg h-[67px]"
  >
    <div class="flex items-center">
      <p class="uppercase font-bold text-2xl text-white">
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
      <div class="flex gap-10 items-center">
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

        <UButton label="Dang nhap" @click="showLogin"></UButton>
      </div>
    </div>
  </header>
</template>

<script setup>
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
