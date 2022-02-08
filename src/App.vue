<script>
import {
  BadgeCheckIcon,
  Circle
} from '@heroicons/vue/outline';
export default {
  components: {
    BadgeCheckIcon
  },
};
</script>

<template>
<div class="flex w-screen h-screen">
  <div class="bg-gray-100 h-full w-1/4">
    <!-- name bar -->
    <div class="flex p-5">
      <div class="h-16 w-16 bg-red-500 rounded-full shadow-lg shadow-red-500/50"></div>
      <div class="flex flex-col justify-center ml-2">
        <span class="text-black font-bold">Sanjiv Patel</span>
        <span class="text-black font-semibold text-xs">sanjiv.patel@ui.com</span>
      </div>
    </div>

    <!-- menu -->
    <div class="flex flex-col">
      <!-- menu heading  -->
      <div class="font-bold text-lg p-5">Menu</div>
      <!-- menu items -->
      <div class="w-full h-16 p-0 flex items-center">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <BadgeCheckIcon class="mx-3 h-8 w-8 font-normal text-red-600"/>
          <!-- name -->
          <div class="text-red-600">Tasks</div>
        </div>
      </div>
      <div class="w-full h-16 p-0 flex items-center" v-for="item in [1,2,3,3,3,2]" :key="item">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600 invisible"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <BadgeCheckIcon class="mx-3 h-8 w-8 font-normal text-gray-400"/>
          <!-- name -->
          <div class="text-gray-400">Tasks</div>
        </div>
      </div>
    </div>

    <!-- menu -->
    <div class="flex flex-col">
      <!-- menu heading  -->
      <div class="font-bold text-lg p-5">Favorites</div>
      <!-- menu items -->
      <div class="w-full h-16 p-0 flex items-center">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600 invisible"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <div class="mx-3 h-8 w-8 font-normal borfer-2"></div>
          <!-- name -->
          <div class="text-gray-400">Rescehedule Design</div>
        </div>
      </div>
    </div>

  </div>
  <div class="bg-white border-r border-l w-1/2"></div>
  <div class="w-1/4 h-full"></div>
</div>
</template>

<style>

</style>
