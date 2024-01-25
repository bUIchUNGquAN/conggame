<template>
  <div
    class="bg-slate-800 rounded-lg shadow-lg w-full md:w-60 h-auto md:h-72 gap-4"
  >
    <div class="py-3 px-3">
      <div v-for="(x, index) in list" :key="index" class="grid grid-cols gap-2">
        <div class="flex flex-cols relative">
          <img
            class="rounded-lg hover:shadow-lg hover:opacity-50 cursor-pointer w-full"
            :src="x.imgUrl"
            alt=""
          />
          <UButton
            label="Ktal"
            color="red"
            class="hover:animate-ping overflow-hidden w-12 absolute top-[50%] left-[50%] transform -translate-x-1/2 -translate-y-1/2 scale-x-150 md:transform-none"
            :src="x.imgUrl"
          ></UButton>
        </div>

        <div class="flex flex-wrap gap-y-4">
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
    <div class="flex flex-cols items-center md:absolute md:right-[3%]">
      <MainBodyOnline />
    </div>
  </div>
</template>

<script setup>
const list = ref([
  {
    imgUrl:
      "https://images2.thanhnien.vn/528068263637045248/2023/11/7/fortnite-og-1699326064259616824163.jpg",
    name: "PUBG Sezon Finali Turmuvasi",
    cois: "500 ga coin",
    modu: "5v5",
  },
]);
</script>
