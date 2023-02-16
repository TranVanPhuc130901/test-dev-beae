<template>
<div class="flex items-center justify-center mt-5">
    <div v-for="list in ListTitle" :class="{'active': list.IsActive}"  :key="list.id" class="tab-group w-[300px] h-[200px] cursor-pointer flex items-center justify-center rounded-[14px_14px_0_0]">
        <div class="tab-item w-[235px] h-[140px] flex flex-col items-center justify-center rounded-lg shadow-[ 0px_0px_27px_rgba(0, 0, 0, 0.05)] bg-white" >
            <div class="tab-item_img w-[58px] h-[58px] flex items-center justify-center rounded-full">
            <img :src="require(`../../assets/${list.urlImg}`)" alt="">
            </div>
            <div class="tab-item_title text-[21px]">{{list.title}}</div>
        </div>
    </div>
</div>
</template>
<script>
export default {
    methods: {
        
    },
    data() {
        return {
            ListTitle: [
                {
                    id: 1,
                    urlImg: 'colors.svg',
                    title: 'Pencils',
                    IsActive: true,
                },
                {
                    id: 2,
                    urlImg: 'marker.png',
                    title: 'Markers',
                    IsActive: false,
                },
                {
                    id: 3,
                    urlImg: 'colors.svg',
                    title: 'Drawing Colors',
                    IsActive: false,
                },
                {
                    id: 4,
                    urlImg: 'notebook.png',
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
    .active{background: #f4f4f4;}
</style>