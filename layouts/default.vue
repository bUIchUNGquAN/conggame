<template>
  <div class="bg-slate-500 min-h-screen">
    <!-- main -->

    <div
      class="fixed flex flex-col justify-end z-[55] end-0 right-0 top-0 bottom-auto w-full sm:w-96"
    ></div>

    <div class="lg:w-full bg-slate-800 rounded-lg shadow-lg mx-auto">
      <MainHead />

      <!-- menu -->
      <div
        class="mx-auto px-4 sm:px-6 lg:px-8 max-w-7xl grid grid-cols-12 gap-0 min-h-[calc(100%-var(--header-size)-var(--footer-size))]"
      >
        <div
          class="bg-slate-900 xl:col-span-2 md:col-span-3 col-span-12 md:block hidden md:sticky md:top-[var(--header-size)] md:max-h-[calc(100vh-var(--header-size)-var(--footer-size))] md:overflow-y-auto py-4"
        >
          <MainMenu></MainMenu>
        </div>
        <!-- body -->
        <div
          class="xl:col-span-8 md:col-span-9 col-span-12 lg:pl-12 md:pl-8 bg-slate-900"
        >
          <MainBodyMain></MainBodyMain>
        </div>
        <!-- chat -->
        <div
          class="xl:col-span-2 md:col-span-3 col-span-12 md:block hidden md:sticky md:top-[var(--header-size)] md:max-h-[calc(100vh-var(--header-size)-var(--footer-size))] md:overflow-y-auto py-4"
        >
          <MainChatfienChat></MainChatfienChat>
        </div>
      </div>
    </div>
  </div>
</template>
