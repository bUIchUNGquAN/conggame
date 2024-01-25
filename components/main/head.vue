<template>
  <header class="sticky top-0 z-50 dark:bg-transparent backdrop-blur-xl">
    <div
      class="mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl flex items-center h-[var(--header-size)] max-h-[var(--header-size)]"
    >
      <div class="flex items-center md:hidden mr-2">
        <UIcon
          name="i-bx-menu-alt-left"
          dynamic
          class="w-7 h-7 cursor-pointer"
        />
      </div>
      <div class="flex items-center mr-auto gap-28">
        <div class="flex items-center">
          <p class="uppercase font-bold text-xl text-white">
            Gamer
            <span class="uppercase font-bold text-xl text-red-900"> arena</span>
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
      </div>
      <div class="flex justify-end items-center">
        <div class="flex items-center ml-1">
          <UIcon
            name="i-bx-credit-card"
            dynamic
            color="white"
            @click="showNotification"
          />
          <div class="flex items-center ml-1">
            <UIcon name="i-bxs-comment-dots" dynamic color="white" />
          </div>
          <div class="flex items-center ml-1">
            <UIcon name="i-bx-bell" dynamic color="white" />
          </div>
          <div class="flex items-center ml-1">
            <UButton
              label="Dang nhap"
              @click="showLogin"
              class="focus:outline-none focus-visible:outline-0 disabled:cursor-not-allowed disabled:opacity-75 flex-shrink-0 font-medium rounded-md text-sm gap-x-1.5 px-2.5 py-1.5 shadow-sm ring-1 ring-inset ring-gray-300 dark:ring-gray-700 text-gray-700 dark:text-gray-200 bg-gray-50 hover:bg-gray-100 disabled:bg-gray-50 dark:bg-gray-800 dark:hover:bg-gray-700/50 dark:disabled:bg-gray-800 focus-visible:ring-2 focus-visible:ring-primary-500 dark:focus-visible:ring-primary-400 inline-flex items-center"
            ></UButton>
          </div>
        </div>
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
