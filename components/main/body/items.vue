<template>
  <div
    class="bg-slate-800 rounded-lg shadow-lg w-full md:w-60 h-auto md:h-72 gap-4"
  >
    <div class="py-3 px-3">
      <div v-for="(x, index) in list" :key="index" class="grid grid-cols gap-2">
        <div class="flex flex-cols">
          <img
            class="rounded-lg hover:shadow-lg hover:opacity-50 cursor-pointer w-full"
            :src="x.imgUrl"
            alt=""
          />
          <UButton
            label="Pc cone"
            color="red"
            class="md:absolute md:top-[40%] md:left-[4%] md:left-[5%]"
            >Pc</UButton
          >
        </div>
        <div
          class="w-12 h-14 bg-slate-800 rounded-lg md:absolute md:top-[22%] md:right-[60%] md:top-[40%] md:right-[22%]"
        >
          <p class="text-white font-bold leading-6 text-center">
            21 <span class="text-sm"> Diem</span>
          </p>
        </div>
        <div
          class="w-12 h-6 bg-slate-800 rounded-lg md:absolute md:top-[38%] md:right-[60%] md:top-[58%] md:right-[22%]"
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
            <p class="text-gray-500 font-bold text-sm">
              Giriss Bedelo : <span class="text-white">{{ x.cois }} </span>
            </p>
            <div class="grid grid-cols-2 gap-9">
              <p class="text-gray-500 font-bold text-sm text-center">
                Toplam Odul <span class="text-white">{{ x.cois }}</span>
              </p>
              <p class="text-gray-500 font-bold text-sm text-center">
                Oyun Odul <span class="text-white">{{ x.modu }}</span>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-cols md:absolute md:left-[3%]">
      <MainBodyOnline />
    </div>
  </div>
</template>

<script setup>
const list = ref([
  {
    imgUrl:
      "https://images2.thanhnien.vn/528068263637045248/2023/11/7/fortnite-og-1699326064259616824163.jpg",
    name: "Fortnite en iyiler turnuvası",
    cois: "250 ga coin",
    modu: "5v5",
  },
]);
</script>
