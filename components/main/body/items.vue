<template>
    <div class="bg-slate-700 rounded-lg shadow-lg rounded-lg w-60 h-72 gap-4">
        <div class="lg:py-3 px-3 ">
            <div v-for="(x,index) in list" :key="x.name" class="grid grid-cols gap-x-6 ">
                <img class="rounded-lg" :src="x.imgUrl" alt="">
                <div class="flex min-w-0 gap-x-4">
                    <UIcon name="i-bx-bell" dynamic/>                        
                    <p class="text-white text-sm font-bold">{{ x.name }}</p>
                </div>
            </div> 
          </div>
        </div>
</template>

<script setup>
    const list=ref([
        {
            imgUrl:'https://images2.thanhnien.vn/528068263637045248/2023/11/7/fortnite-og-1699326064259616824163.jpg',
            name:'Forinite en iyiler turnersi',
            cois:'250 ga coin',
            modu:'5v5'
        },
       
    ])
</script>