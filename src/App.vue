<script>
import {
  BadgeCheckIcon,
  PlusIcon,
  SparklesIcon,
  DotsHorizontalIcon,
  SearchIcon,
} from '@heroicons/vue/outline';
export default {
  components: {
    BadgeCheckIcon,
    PlusIcon,
    SparklesIcon,
    DotsHorizontalIcon,
    SearchIcon,
  },
};
</script>

<template>
<div class="flex mx-auto container">
  <div class="bg-gray-100 h-screen w-1/4 relative overflow-auto no-scroll-bar p-0">
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
          <div class="mx-3 h-6 w-6 font-normal border-2 border-yellow-400 rounded-full"></div>
          <!-- name -->
          <div class="text-gray-400">Rescehedule Design</div>
        </div>
      </div>
      <div class="w-full h-16 p-0 flex items-center">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600 invisible"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <div class="mx-3 h-6 w-6 font-normal border-2 border-cyan-400 rounded-full"></div>
          <!-- name -->
          <div class="text-gray-400">Layout Scaffolding</div>
        </div>
      </div>
      <div class="w-full h-16 p-0 flex items-center">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600 invisible"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <div class="mx-3 h-6 w-6 font-normal border-2 border-green-400 rounded-full"></div>
          <!-- name -->
          <div class="text-gray-400">UX Testing</div>
        </div>
      </div>
      <div class="w-full h-16 p-0 flex items-center">
        <span class="h-12 w-2 rounded-tr-full rounded-br-full bg-red-600 invisible"></span>
        <div class="flex w-full items-center">
          <!-- icon -->
          <div class="mx-3 h-6 w-6 font-normal border-2 border-purple-400 rounded-full"></div>
          <!-- name -->
          <div class="text-gray-400">Scaling</div>
        </div>
      </div>
    </div>

    <!-- footer -->
    <div class="p-5 flex flex-col">
      <div class="h-16 w-16 bg-gradient-to-r from-red-500 via-red-600 to-red-600 rounded-full flex items-center justify-center">
        <PlusIcon class="text-white h-8 w-8" />
      </div>
    </div>

    <div class="text-gray-400 mt-5 font-bold text-sm absolute bottom-3 left-5">&#169; 2022 UI/UX Designs ui.com</div>

  </div>
  <div class="bg-white border-r border-l w-1/2 h-screen overflow-auto no-scroll-bar">
    <!-- greeting -->
    <div class="flex p-5 justify-between">
      <p class="text-3xl font-bold font-sans">Hi Sanjiv</p>
      <div class="flex items-center">
        <span class="font-sans text-gray-400 text-sm font-bold mr-3">15% task completions</span>
        <div class="w-[100px] bg-gray-200 rounded-full h-2.5">
          <div class="bg-red-600 h-2.5 rounded-full" style="width: 45%"></div>
        </div>
      </div>
    </div>

    <!-- cards 8th Feb 2022 -->
    <div class="p-5 flex flex-nowrap space-x-2 w-full overflow-x-auto no-scroll-bar cursor-pointer">
      <div class="flex-none flex h-80 w-80 bg-gradient-to-r from-red-500 via-red-600 to-red-600 rounded-xl p-10">
        <!-- card content -->
        <div class="h-ful w-full rounded-2xl flex flex-col">
          <div class="flex justify-between">
            <div class="h-20 w-20 bg-red-800 rounded-2xl flex justify-center items-center">
              <SparklesIcon class="h-12 w-12 text-gray-100"/>
            </div>
            <DotsHorizontalIcon class="h-10 w-10 text-gray-100"/>
          </div>
          <div class="text-2xl font-bold text-white mt-4">
            R&D for new Banking Mobile App
          </div>
          <div class="relative mt-4 flex">
            <div class="absolute border-2 border-white bg-yellow-400 h-12 w-12 rounded-full"></div>
            <div class="absolute left-8 border-2 border-white bg-yellow-400 h-12 w-12 rounded-full"></div>
            <div class="absolute left-16 border-2 border-white bg-yellow-400 h-12 w-12 rounded-full"></div>
          </div>
        </div>
      </div>
      <div class="flex-none flex h-80 w-80 bg-gradient-to-r from-purple-500 via-purple-600 to-purple-700 rounded-xl p-10" v-for="item in [1,2,3,3,3,2]" :key="item">
        <div class="h-ful w-full rounded-2xl flex flex-col">
          <div class="flex justify-between">
            <div class="h-20 w-20 bg-purple-800 rounded-2xl flex justify-center items-center">
              <SparklesIcon class="h-12 w-12 text-gray-100"/>
            </div>
            <DotsHorizontalIcon class="h-10 w-10 text-gray-100"/>
          </div>
          <div class="text-2xl font-bold text-white mt-4">
            R&D for new Banking Mobile App
          </div>
          <div class="relative mt-4 flex">
            <div class="absolute border-2 border-white bg-cyan-400 h-12 w-12 rounded-full"></div>
            <div class="absolute left-8 border-2 border-white bg-green-400 h-12 w-12 rounded-full"></div>
            <div class="absolute left-16 border-2 border-white bg-yellow-400 h-12 w-12 rounded-full"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- tabs 9th Feb 2022 -->
    <!-- heading -->
    <div class="flex p-5 justify-between">
      <h2 class="text-3xl font-bold">Monthly Tasks</h2>
      <!-- buttons -->
      <div class="flex space-x-2">
        <button class="font-semibold p-2 h-9 text-sm rounded-full w-20 bg-gray-300 text-black">Archive</button>
        <button class="font-semibold p-2 h-9 text-sm rounded-full w-20 bg-purple-700 text-white flex items-center justify-around">
          <PlusIcon class="h-5 w-5 text-white"/>
          <span>New</span>
        </button>
      </div>
    </div>

    <!-- tabs -->
    <div class="w-full flex flex-col overflow-auto">
      <div class="flex justify-between h-10 shadow-sm px-5 mt-10">
        <div class="flex space-x-5">
          <div class="cursor-pointer text-lg p-1 font-semibold font-sans text-purple-700 h-10 border-b-2 border-purple-700">Archived</div>
          <div class="cursor-pointer text-lg p-1 font-semibold font-sans text-gray-300 h-10">Pending</div>
          <div class="cursor-pointer text-lg p-1 font-semibold font-sans text-gray-300 h-10">Complete</div>
        </div>
        <div class="flex space-x-2 text-gray-400 relative mb-2">
          <SearchIcon class="h-6 w-6 absolute left-5 top-2 z-10"/>
          <input class="w-36 px-10 rounded-full h-10 focus-within:w-48 transform duration-500 translate-x-1" placeholder="Search"/>
        </div>
      </div>
      <!-- tab lists -->
      <div class="px-5 py-5 w-full flex flex-col divide-y">
        <div class="py-1 text-lg font-semibold font-sans text-gray-300 h-10">Today</div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-red-500/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-red-600 rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-purple-500/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-purple-600 rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-orange-500/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-orange-400 rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
      </div>
      <div class="px-5 py-5 h-full w-full flex flex-col divide-y">
        <div class="py-1 text-lg font-semibold font-sans text-gray-300 h-10">Tomorrow</div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-purple-500/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-purple-800 rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-gray-900/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-black rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
        <div class="py-3 flex items-center space-x-2">
          <div class="shadow-lg shadow-gray-900/60 h-24 w-24 flex-grow-0 flex-shrink-0 bg-black rounded-3xl flex items-center justify-center">
            <BadgeCheckIcon class="h-16 w-16 text-white" />
          </div>
          <div class="flex flex-col">
            <h3 class="text-black text-2xl font-bold">Uber Story</h3>
            <p class="text-gray-400 text-sm w-80">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            </p>
          </div>
          <div class="relative flex items-center bg-black">
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-0"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-8"></div>
            <div class="h-12 w-12 absolute border-2 bg-sky-500 rounded-full left-16"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="w-1/4 h-full"></div>
</div>
</template>

<style>
body {
  @apply font-sans text-black
}
</style>
