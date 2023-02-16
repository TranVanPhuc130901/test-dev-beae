<template >
<div class="flex justify-between">
        <div class="w-[224px] h-[320px] rounded-[18px] bg-white cursor-pointer" v-for="product in ListProduct" :key="product.id">
        <div class="">
            <div class="flex items-center justify-center">
                <img class="" :src="require(`../../assets/${product.img}`)" alt="">
            </div>
            <div class="text-center">
                <div class="text-sm">{{product.title}}</div></div>
                <div class="flex items-center gap-[11px] justify-center">
                    <div class="text-base">{{product.price}}</div>
                    <del class="text-sm text-[#727272]">{{product.promotion}}</del>
                </div>
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
             ListProduct:[
                {
                    id: 1,
                    img: 'pen-img111.png',
                    title: 'Aero Mechanical Pencil',
                    price: '$99.00', 
                    promotion: '$125.00'
                },
                 {
                    id: 2,
                    img: 'pen-img112.png',
                    title: 'Castell Mechanical Pencil',
                    price: '$75.00', 
                    promotion: '$99.00'
                },
                 {
                    id: 3,
                    img: 'pen-img1133.png',
                    title: 'Architect Choice Pencil',
                     price: '$45.00', 
                    promotion: '$70.00'
                },
            ]
        }
    },
}
</script>
<style >
    
</style>