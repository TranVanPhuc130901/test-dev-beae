<template>
<div class="flex flex-col w-full items-center justify-center mt-5 bg-[#f4f4f4]">
   <div class="w-full">
     <div class="p-[10px] tab-group w-full h-[80px] cursor-pointer flex items-center justify-center rounded-[14px_14px_0_0]">
        <div @click="IsShow = !IsShow; showImg = !showImg" class="tab-item w-full px-[30px] py-[17px] h-full flex items-center justify-between rounded-lg shadow-[ 0px_0px_27px_rgba(0, 0, 0, 0.05)] bg-white gap-5" >
           <div class="flex items-center justify-center gap-3 rounded-full">
             <div class="tab-item_img w-[50px] h-[50px] flex items-center justify-center rounded-full">
                <img class="w-[27px] h-[27px]" src="../../assets/pencilsMoblie.svg" alt="">
            </div>
            <div class="tab-item_title text-[21px]">Pencils</div>
           </div>
             <img v-if="!showImg" class="" src="../../assets/down.png" alt="">
             <img v-if="showImg" class="" src="../../assets/up.png" alt="">
        </div>
    </div>
        <GalleryDetailMobile v-if="IsShow"></GalleryDetailMobile>
   </div>
     <div  class="p-[10px] tab-group w-full h-[80px] cursor-pointer flex items-center justify-center rounded-[14px_14px_0_0]">
        <div class="tab-item w-full px-[30px] py-[17px] h-full flex items-center justify-between rounded-lg shadow-[ 0px_0px_27px_rgba(0, 0, 0, 0.05)] bg-white gap-5" >
           <div class="flex items-center justify-center gap-3 rounded-full">
             <div class="tab-item_img w-[50px] h-[50px] flex items-center justify-center rounded-full">
                <img class="w-[27px] h-[27px]" src="../../assets/markerMobile.svg" alt="">
            </div>
            <div class="tab-item_title text-[21px]">Markers</div>
           </div>
             <img class="" src="../../assets/down.png" alt="">
        </div>
    </div>
     <div  class="p-[10px] tab-group w-full h-[80px] cursor-pointer flex items-center justify-center rounded-[14px_14px_0_0]">
        <div class="tab-item w-full px-[30px] py-[17px] h-full flex items-center justify-between rounded-lg shadow-[ 0px_0px_27px_rgba(0, 0, 0, 0.05)] bg-white gap-5" >
           <div class="flex items-center justify-center gap-3 rounded-full">
             <div class="tab-item_img w-[50px] h-[50px] flex items-center justify-center rounded-full">
                <img class="w-[27px] h-[27px]" src="../../assets/colorsMoblie.svg" alt="">
            </div>
            <div class="tab-item_title text-[21px]">Drawing Colors</div>
           </div>
             <img class="" src="../../assets/down.png" alt="">
        </div>
    </div>
     <div  class="p-[10px] tab-group w-full h-[80px] cursor-pointer flex items-center justify-center rounded-[14px_14px_0_0]">
        <div class="tab-item w-full px-[30px] py-[17px] h-full flex items-center justify-between rounded-lg shadow-[ 0px_0px_27px_rgba(0, 0, 0, 0.05)] bg-white gap-5" >
           <div class="flex items-center justify-center gap-3 rounded-full">
             <div class="tab-item_img w-[50px] h-[50px] flex items-center justify-center rounded-full">
                <img class="w-[27px] h-[27px]" src="../../assets/noteMoblie.svg" alt="">
            </div>
            <div class="tab-item_title text-[21px]">Notebooks</div>
           </div>
             <img class="" src="../../assets/down.png" alt="">
        </div>
    </div>
    
</div>
</template>
<script>
import GalleryDetailMobile from '../pages/gallery/GalleryDetailMobile.vue'
export default {
    components: {
        GalleryDetailMobile
    },
    methods: {
        
    },
    data() {
        return {
            IsShow: true,
            showImg: true,
            ListTitle: [
                {
                    id: 1,
                    urlImg: 'pencilsMoblie.svg',
                    title: 'Pencils',
                    IsActive: true,
                },
                {
                    id: 2,
                    urlImg: 'markerMobile.svg',
                    title: 'Markers',
                    IsActive: false,
                },
                {
                    id: 3,
                    urlImg: 'colorsMoblie.svg',
                    title: 'Drawing Colors',
                    IsActive: false,
                },
                {
                    id: 4,
                    urlImg: 'noteMoblie.svg',
                    title: 'Notebooks',
                    IsActive: false,
                },

            ],
           
        }
    },
}
</script>
<style scoped>
    .tab-item_img{
        background: #F4F4F4;
    }
    .tab-item_title{color: #181818;}
    .active{}
</style>