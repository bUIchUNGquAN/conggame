<template>
  <div class="relative">
    <img src="/assets/img/body.jpg" class="opacity-50 w-full" />
    <div class="grid grid-rows-1 md:grid-rows-4 gap-4 md:flex md:flex-wrap">
      <div
        class="absolute top-[25%] left-[10%] grid grid-rows-1 gap-3 md:w-1/2"
      >
        <img
          src="https://cdn.pixabay.com/photo/2021/08/28/09/27/pubg-mobile-logo-6580513_640.png"
          class="w-24 h-12"
          alt=""
        />

        <p class="text-white leading-6 font-bold text-xl">
          Game lau nap la bu.
        </p>
        <div class="flex flex-col md:flex-row">
          <UButton label="Turnuvaya" color="red" size="xl"
            >choi game nhanh</UButton
          >
          <UButton
            label="Detayli Bilgi"
            color=""
            variant="ghost"
            class="text-white"
            size="xl"
            >Detayli Bilgi</UButton
          >
        </div>
      </div>
      <!-- <div
        class="py-2 grid grid-rows-1 gap-5 absolute top-[70%] left-[10%] w-full md:w-auto"
      >
        <p class="font-bold text-white text-2xl">Populer Turnuvalar</p>
        <div class="flex flex-wrap items-center justify-between gap-6">
          <div class="flex-1 md:inline-flex">
            <MainBodyItems />
          </div>
          <div class="flex-1 md:inline-flex">
            <MainBodyItems2 />
          </div>
          <div class="flex-1 md:inline-flex">
            <MainBodyItems3 />
          </div> -->
    </div>
  </div>
</template>
