<template>
  <div class="bg-slate-500 h-screen">
    <!-- main -->
    <div class="w-[90%] bg-slate-800 rounded-lg absolute left-[5%] shadow-lg">
      <MainHead></MainHead>
      <!-- menu -->
      <div class="flex flex-cols">
        <div class="flex-none w-1/5 h-screen bg-slate-900">
          <MainMenu></MainMenu>
        </div>
        <!-- body -->
        <div class="grow w-2/4 h-screen bg-slate-700">
          <MainMain></MainMain>
        </div>
        <!-- chat -->
        <div class="flex-none w-1/5 h-screen bg-slate-900 float-left">
          <MainChat></MainChat>
        </div>
      </div>
    </div>
  </div>
</template>
