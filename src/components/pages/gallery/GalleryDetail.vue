<template>
    <div class=" bg-[#f4f4f4] rounded-[0_0_25px_25px]">
        <div class="p-[40px_50px] flex gap-[38px]">
            <div class="w-[calc(100%-750px)]">
                <div class="text-[21px] text-[#000] mb-[20px]">Graphite Artist Quality Fine Art Drawing and Sketching Pencils Replaceable Nib Pencils. </div>
                <ul class="mb-[35px] ml-5 list-disc font-[600]">
                    <li class="text-lg">MECHANICAL PENCILS </li>
                    <li class="text-lg">ARCHITECT'S CHOICE</li>    
                    <li class="text-lg">EXECUTIVE PENCILS</li>
                    <li class="text-lg">ENGRAVABLE PENCILS</li> 
                </ul>
                <button class="w-[120px] h-[50px] bg-[#F4B840] text-[#fff] text-sm font-bold rounded-[5px]">Shop All</button>
            </div>
        <div class="w-[712px] ">
            <div class="flex rounded-[18px] items-center justify-between border-[3px] border-[#fff] mb-5">
                <div class="w-[200px] text-4xl font-bold text-[#F4B840] bg-white rounded-[18px_0_0_18px] p-[13px_28px_13px_40px]">25% off</div>
                <div class="w-[calc(100%-200px)] pl-[24px] text-[25px]">Offer Applicable on All Our Pencils</div>
            </div>
            <TheTabProduct></TheTabProduct>
        </div>
        </div>
    </div>
</template>

<script>
import TheTabProduct from '../../base/TheTabProduct.vue'
export default {
    components: {TheTabProduct},
}
</script>
<style>
    
</style>