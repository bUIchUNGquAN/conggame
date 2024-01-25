<template>
    <div class="py-1 px-4 lg:px-8">
        <div class="border-b shadow-lg divide-y-4 divide-slate-400/25 py-2">
      <p class="text-white text-2xl">Chat</p>
    </div>
    <div class="py-3">
      <li v-for="(x,index) in list" :key="index" class="flex justify-between py-2">
        <div class="flex flex-cols gap-4">
          <UAvatar :src="x.imgrul" />
          <div class="grid grid-rows-1 gap-x-2">
            <p class="text-white font-bold">
              {{x.name}}
              <UIcon name="i-bxs-circle" dynamic color="green" />
            </p>
            <p class="text-gray-400 text-sm italic ">{{ x.statut }}</p>
            <p class="text-slate-300 text-sm leading-6">{{ x.text }}</p>
          </div>
        </div>
      </li>
    </div>
    <div class="container mx-auto py-2 px-1">
      <MainChatfienItemsSolo />
    </div>
    <div class="py-5 px-3">
      <div class="flex flex-cols gap-4">
                <UAvatar src="https://genk.mediacdn.vn/thumb_w/640/2016/best-photos-2016-natgeo-national-geographic-7-5846f70467192-880-1481173142742.jpg" />
                <div class="grid grid-rows-1  gap-x-2">
                    <p class="text-white font-bold flex flex-cols gap-3">
                        <UIcon name="i-bxs-circle" dynamic color="green" />
                        <div class="bg-slate-700 w-[50px] shadow-2xl rounded-lg">
                            <p class="text-sm text-white text-center font-bold leading-5">
                                Team
                            </p>
                        </div>
                    </p>    
                    <p class="text-gray-400 text-sm italic "> 2 Daika once</p>
                    <p class="text-slate-300 text-sm text-white leading-6  ">bak cevirdi suan gordun mu suan cevirdi :ddd</p>  
                </div>              
            </div>
            <div class="py-2 flex flex-cols gap-3">
                <UAvatar src="https://genk.mediacdn.vn/thumb_w/640/2016/best-photos-2016-natgeo-national-geographic-7-5846f70467192-880-1481173142742.jpg" />
                <div class="grid grid-rows-1  gap-x-2">
                    <p class="text-white font-bold flex flex-cols gap-3">skt
                        <UIcon name="i-bxs-circle" dynamic color="green" />
                        <div class="bg-slate-700 w-[50px] shadow-2xl rounded-lg">
                            <p class="text-sm text-white text-center font-bold leading-5">
                                Team
                            </p>
                        </div>
                    </p>    
                    <p class="text-gray-400 text-sm italic "> 2 Daika once</p>
                    <p class="text-slate-300 text-sm text-white leading-6  ">bak cevirdi suan gordun mu suan cevirdi :ddd</p>  
                </div>              
            </div>
            <div class="py-1 flex flex-cols gap-3">
                <UAvatar src="https://static-images.vnncdn.net/files/publish/2022/9/3/bien-vo-cuc-thai-binh-346.jpeg" />
                <div class="grid grid-rows-1 gap-x-2">
                    <p class="text-white font-bold">Chapper
                        <UIcon name="i-bxs-circle" dynamic color="green" />
                    </p>
                    <p class="text-gray-400 text-sm italic ">Duello istegi</p>
                    <p class="text-slate-300 text-sm leading-6 text-white ">skt faker yine yargi pesinde adam mg icinden gecti</p>  
                </div>              
            </div>
        </div>
        <div class="container mx-auto py-2 px-1">
      <MainChatfienItemsSolo/>
    </div>
    </div>
</template>

<script setup>
    const list= ref([
        {
            imgrul:'https://genk.mediacdn.vn/thumb_w/640/2016/best-photos-2016-natgeo-national-geographic-7-5846f70467192-880-1481173142742.jpg',
            name:'The Player1',
            statut:'5 Daika once',
            text:'>buralar cok duttluk olmus neden boyle olmus? hodi bunrun aratramasmi yapalm',
            lastSeen:null
        },
        {
            imgrul:'https://media.baoquangninh.vn/upload/image/202310/medium/2137171_f1207af841cbfc6683b03f4d1fdab7ce.jpg',
            name:'Chapps ',
            statut:'3 Daika once',
            text:'>buralar cok duttluk olmus neden boyle olmus? hodi bunrun aratramasmi yapalm',
            lastSeen:null
        },
        {
            imgrul:'https://static-images.vnncdn.net/files/publish/2022/9/3/bien-vo-cuc-thai-binh-346.jpeg',
            name:'skt telecom',
            statut:'2 Daika once',
            text:'skt faker yine yargi pesinde adam mg icinden gecti',
            lastSeen:null
        },
        {
            imgrul:'https://www.elle.vn/wp-content/uploads/2017/04/19/anh-nude-nghe-thuat-elle-viet-nam-26.jpg',
            name:'mg3321',
            statut:'2 Daika once',
            text:'ahahahahaha mg bence bu moci cevirin',
            lastSeen:null
        },
    ])
</script>