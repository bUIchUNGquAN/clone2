<template>
 
  <div class="bg-slate-500 h-screen">
    <!-- main -->
    <div class="lg:w-[100%] bg-slate-800 rounded-lg   shadow-lg">
      <MainHead></MainHead>
      <!-- menu -->
      <div class="lg:flex flex-cols ">
        <div class="w-1/5 h-screen bg-slate-900">
          <MainMenu></MainMenu>
          
        </div>
        <!-- body -->
        <div class="grow w-2/4 h-screen bg-slate-700">
          <MainBodyMain></MainBodyMain>
          
        </div>
        <!-- chat -->
        <div class="w-1/5 h-screen bg-slate-900 float-left">
          <MainChatfienChat></MainChatfienChat>
          
        </div>
      </div>
    </div>
  </div>
</template>
