<template>
  <div class="mb-4">
    <div class="grid grid-rows-3 gap-4 lg:grid-rows-3 lg:gap-8">
      <div class="grid grid-rows-6 gap-4">
        <p class="uppercase font-bold text-white">menu</p>
        <div class="flex flex-cols gap-2">
          <UIcon name="i-bx-cake" dynamic color="white" class="w-6 h-6" />
          <p
            class="font-bold text-xm text-white cursor-pointer hover:text-black"
          >
            Arane
          </p>
        </div>
        <div class="flex flex-cols gap-2">
          <UIcon name="i-bx-knife" dynamic color="white" class="w-6 h-6" />
          <p
            class="font-bold text-xm text-white cursor-pointer hover:text-black"
          >
            Duellolar
          </p>
        </div>
        <div class="flex flex-cols gap-2">
          <UIcon name="i-bx-medal" dynamic color="white" class="w-6 h-6" />
          <p
            class="font-bold text-xm text-white cursor-pointer hover:text-black"
          >
            Turnuvalar
          </p>
        </div>
        <div class="flex flex-cols gap-2">
          <UIcon name="i-bx-bell" dynamic color="white" class="w-6 h-6" />
          <p
            class="font-bold text-xm text-white cursor-pointer hover:text-black"
          >
            Bildirimler
          </p>
        </div>
        <div class="flex flex-cols gap-2">
          <UIcon name="i-bxs-hand" dynamic color="white" class="w-6 h-6" />
          <p
            class="font-bold text-xm text-white cursor-pointer hover:text-black"
          >
            Takimlar
          </p>
        </div>
      </div>

      <div class="px-1 py-6 lg:py-0">
        <div class="lg:grid grid-rows-7 gap-2">
          <p class="uppercase font-bold text-white">oyunlar</p>
          <div
            v-for="(x, index) in list"
            :key="index"
            class="flex flex-cols gap-2"
          >
            <UAvatar :src="x.imgrl" />
            <p
              class="font-bold text-xm text-white cursor-pointer hover:text-black"
            >
              {{ x.name }}
            </p>
          </div>
        </div>
      </div>
      <div class="px-2">
        <div class="lg:grid grid-rows-7 gap-2">
          <p class="uppercase font-bold text-white">destek merkezi</p>
          <div class="flex flex-cols gap-2">
            <UAvatar
              src="https://logos-world.net/wp-content/uploads/2023/02/LoL-Symbol.png"
            />
            <p
              class="font-bold text-xm text-white cursor-pointer hover:text-black"
            >
              Yardım & Destek
            </p>
          </div>
          <div class="flex flex-cols gap-2">
            <UAvatar
              src="https://cdn.tgdd.vn/Files/2018/03/23/1076619/fifa-online-4-featured_800x450.jpg"
            />
            <p
              class="font-bold text-xm text-white cursor-pointer hover:text-black"
            >
              S.S.S
            </p>
          </div>
          <div class="flex flex-cols gap-2">
            <UAvatar
              src="https://m.media-amazon.com/images/M/MV5BNzU2YTY2OTgtZGZjZi00MTAyLThlYjUtMWM5ZmYzOGEyOWJhXkEyXkFqcGdeQXVyNTgyNTA4MjM@._V1_FMjpg_UX1000_.jpg"
            />
            <p
              class="font-bold text-xm text-white cursor-pointer hover:text-black"
            >
              Nasul Colsar?
            </p>
          </div>
          <div class="flex flex-cols gap-2">
            <UAvatar
              src="https://upload.wikimedia.org/wikipedia/commons/e/e0/Rocket_League_coverart.jpg"
            />
            <p
              class="font-bold text-xm text-white cursor-pointer hover:text-black"
            >
              Turkce
            </p>
            <UIcon
              name="i-bx-down-arrow-alt"
              color="gray"
              class="grow h-6 absolute left-[14%] cursor-pointer"
              dynamic
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const list = ref([
  {
    imgrl: "https://logos-world.net/wp-content/uploads/2023/02/LoL-Symbol.png",
    name: "League of Legends",
  },
  {
    imgrl:
      "https://cdn.tgdd.vn/Files/2018/03/23/1076619/fifa-online-4-featured_800x450.jpg",
    name: "Fifa 2019",
  },
  {
    imgrl:
      "https://m.media-amazon.com/images/M/MV5BNzU2YTY2OTgtZGZjZi00MTAyLThlYjUtMWM5ZmYzOGEyOWJhXkEyXkFqcGdeQXVyNTgyNTA4MjM@._V1_FMjpg_UX1000_.jpg",
    name: "Fortnite",
  },
  {
    imgrl:
      "https://upload.wikimedia.org/wikipedia/commons/e/e0/Rocket_League_coverart.jpg",
    name: "Rocket League",
  },
  {
    imgrl:
      "https://play-lh.googleusercontent.com/uJM2tbls8q1eNjHN-MYWBAo5ckmNgHXTFnGSUWSkJyEr40H-WFgka0tvFiTFNG4bOJi2",
    name: "Teamfight Tactics",
  },
  {
    imgrl:
      "https://assets-prd.ignimgs.com/2022/01/28/heroes-of-the-storm-button-crop-1643355577739.jpg",
    name: "Heroes of the Storm",
  },
]);
</script>
