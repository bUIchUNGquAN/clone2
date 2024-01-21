<template>
  <div class="bg-slate-500">
    <!-- main -->
    <div class="lg:w-[90%] bg-slate-800 rounded-lg shadow-lg mx-auto">
      <MainHead></MainHead>
      <!-- menu -->
      <div class="lg:flex flex-cols">
        <div class="lg:w-1/5 bg-slate-900">
          <MainMenu></MainMenu>
        </div>
        <!-- body -->
        <div class="grow lg:w-2/4 bg-slate-700">
          <MainBodyMain></MainBodyMain>
        </div>
        <!-- chat -->
        <div class="lg:w-1/5 bg-slate-900 lg:float-left">
          <MainChatfienChat></MainChatfienChat>
        </div>
      </div>
    </div>
  </div>
</template>
