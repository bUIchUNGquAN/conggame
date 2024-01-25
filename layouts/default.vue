<template>
  <div class="bg-slate-500 min-h-screen">
    <!-- main -->

    <MainFormLogin />

    <div class="lg:w-[90%] bg-slate-800 rounded-lg shadow-lg mx-auto">
      <MainHead />

      <!-- menu -->
      <div class="flex flex-cols lg:flex-row">
        <div class="w-full lg:w-1/5 bg-slate-900">
          <MainMenu></MainMenu>
        </div>
        <!-- body -->
        <div class="grow w-full lg:w-2/4 bg-slate-700">
          <MainBodyMain></MainBodyMain>
        </div>
        <!-- chat -->
        <div class="w-full lg:w-1/5 bg-slate-900 mt-4 lg:mt-0">
          <MainChatfienChat></MainChatfienChat>
        </div>
      </div>
    </div>
  </div>
</template>
