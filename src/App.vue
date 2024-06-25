<script setup> 
import { ref, onMounted } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
// import ChevronUp from 'vue-material-design-icons/CheronUp.vue';
// import ChevronDown from 'vue-material-design-icons/CheronDown.vue';
import ChevronRight from 'vue-material-design-icons/ChevronRight.vue';
import ChevronLeft from 'vue-material-design-icons/ChevronLeft.vue';

let openMenu = ref(false)
</script> 
 
<template>
  <div class="
    w-[calc(100%-240px)]
    h-[60px]
    fixed
    right-0
    z-20
    bg-[#101010]
    bg-opacity-80
    flex
    items-center
    justify-between
  ">
    <div class="flex items-center ml-6">
      <button type="button" class="rounded-full bg-black p-[1px] cursor-pointer">
        <ChevronLeft fillColor="#FFFFFF" :size="30" />
      </button>
      <button type="button" class="rounded-full bg-black p-[1px] ml-4 cursor-pointer">
        <ChevronRight fillColor="#FFFFFF" :size="30" />
      </button>
    </div>
    <button class="bg-black hover:bg-[#282828] rounded-full p-0.5 mr-8 mt-0.5 cursor-pointer">
      <div class="flex items-center">
        <img 
          class="rounded-full"
          width="27"
          src="https://yt3.ggpht.com/yti/ANjgQV9RsCIavgycl4O-v2Me-JysEzCpn1Hz0RmLRfPmsHE=s88-c-k-c0x00ffffff-no-rj-mo"
        />
        <div class="text-white test-[14px] ml-1.5 font-semibold">John Weeks Dev</div>
      </div>
    </button>
  </div>
</template> 
