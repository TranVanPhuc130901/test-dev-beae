<template>
<div>
    <div class="max-w-[1200px] mx-auto max-lg:hidden">
        <div class="" v-if="IsShow">
          <TheTabTitle></TheTabTitle>
          <GalleryDetail></GalleryDetail>
        </div>
          <TabDetails v-if="!IsShow"></TabDetails>
          <div class="flex justify-center gap-1 my-2">
            <div @click="IsShow = !IsShow ; IsActive = !IsActive" :class="{'active': IsActive}" class="w-[15px] h-[15px] rounded-full bg-slate-300 cursor-pointer"></div>
            <div @click="IsShow = !IsShow ; IsActive = !IsActive" :class="{'active': !IsActive}" class="w-[15px] h-[15px] rounded-full bg-slate-300 cursor-pointer"></div>
          </div>
  </div>
  <div class="lg:hidden">
    <div>
        <TheTabTitleMobile  v-if="IsShow"></TheTabTitleMobile>
        <div>
          <TabDetailsMobile  v-if="!IsShow"></TabDetailsMobile>
        </div>
    </div>
    <div class="flex justify-center gap-1 my-2">
            <div @click="IsShow = !IsShow ; IsActive = !IsActive" :class="{'active': IsActive}" class="w-[15px] h-[15px] rounded-full bg-slate-300 cursor-pointer"></div>
            <div @click="IsShow = !IsShow ; IsActive = !IsActive" :class="{'active': !IsActive}" class="w-[15px] h-[15px] rounded-full bg-slate-300 cursor-pointer"></div>
    </div>
  </div>
</div>
  
</template>

<script>

import TheTabTitle from '../src/components/base/TheTabTitle.vue'
import GalleryDetail from '../src/components/pages/gallery/GalleryDetail.vue'
import TabDetails from '../src/components/pages/tabs/TabsDetail.vue'
import TabDetailsMobile from '../src/components/pages/tabs/TabDetailsMobile.vue'
import TheTabTitleMobile from '../src/components/base/TheTabTitleMobile.vue'
export default {
  name: 'App',
  components: {
    TheTabTitle,
    GalleryDetail,
     TabDetails,
     TheTabTitleMobile
     ,TabDetailsMobile
  },
  data() {
    return {
      IsActive: true,
      IsShow: true
    }
  },
}
</script>

<style scoped>
 .active{background: #000;}
</style>


