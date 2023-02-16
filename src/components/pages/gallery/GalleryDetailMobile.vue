<template>
    <div class=" bg-[#f4f4f4] rounded-[0_0_25px_25px]">
        <div class="p-[40px_50px] flex flex-wrap gap-[38px]">
            <div class="w-full">
                <div class="text-[21px] text-[#000] mb-[20px]">Graphite Artist Quality Fine Art Drawing and Sketching Pencils Replaceable Nib Pencils. </div>
                <ul class="mb-[35px] ml-5 list-disc font-[600] flex justify-between " >
                    <div>
                        <li class="text-lg max-sm:text-sm">MECHANICAL PENCILS </li>
                        <li class="text-lg max-sm:text-sm">ARCHITECT'S CHOICE</li>    
                    </div>
                    <div>
                        <li class="text-lg max-sm:text-sm">EXECUTIVE PENCILS</li>
                        <li class="text-lg max-sm:text-sm">ENGRAVABLE PENCILS</li>
                    </div>
                </ul>
                <button class="w-[120px] h-[50px] bg-[#F4B840] text-[#fff] text-sm font-bold rounded-[5px]">Shop All</button>
            </div>
        <div class="w-full ">
            <div class="flex rounded-[18px] items-center justify-between border-[3px] border-[#fff] mb-5 p-5">
                <div class="w-[200px] text-4xl font-bold text-[#F4B840] bg-white rounded-[18px_0_0_18px] p-[13px_28px_13px_40px]">25% off</div>
                <div class="w-[calc(100%-200px)] pl-[24px] text-[25px] max-sm: text-base">Offer Applicable on All Our Pencils</div>
            </div>
            <TheTabProductMoblie></TheTabProductMoblie>
        </div>
        </div>
    </div>
</template>

<script>
import TheTabProductMoblie from '../../base/TheTabProductMoblie.vue'
export default {
    components: {TheTabProductMoblie},
}
</script>
<style>
    
</style>