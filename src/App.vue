<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Header from './components/Header.vue'
import Sidebar from './components/Sidebar.vue'
import Topics from './components/Topics.vue'
</script>

<template>
  <div class="w-screen h-screen flex flex-col relative  text-gray-800 dark">
    <Header></Header>
    <Sidebar></Sidebar>
    <div class="pt-12 pl-20 w-full h-full bg-gray-100  dark:bg-dark-600 dark:text-gray-100">
      <Topics></Topics>
      <div class="catalogue grid grid-cols-3 lg:grid-cols-5 justify-start gap-4 p-4 pt-14 w-full h-full overflow-y-auto overflow-x-hidden">
        
        <div class="relative" v-for="post in [1,2,3,4,5,6,7,8,9,10,11,12, 13,14,15]" :key="post+'sf'">
          <div  class=" h-70 hover:absolute hover:top-0 hover:right-0 hover:h-93 dark:bg-dark-600 bg-white flex flex-col cursor-pointer transform transition-transform hover:shadow-lg hover:z-10 hover:scale-110 group">
          <div class="image w-full h-2/4 group-hover:h-2/5 bg-gray-400 relative flex flex-col">
            
            <img class="w-full h-full object-cover" :key="'img_'+post" :src="`https://picsum.photos/20${post}/20${post}`" alt="">
            <p class="absolute px-2 bg-black text-white bg-opacity-75 bottom-1 right-1 ">16:03</p>
          </div>
          <div class="flex p-2">
            <div class="w-10 h-9 rounded-full bg-red-400">
            </div>
            <div class="w-full flex flex-col pl-2">
              <p class="text-sm font-semibold mb-2">Occaecat cillum laborum in labore ullamco occaecat excepteur commodo.</p>
              <div class="flex  items-center text-gray-400">
                <p>LUK3D</p>
                <div class="w-4 h-4 ml-2">
                  <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false" class="style-scope yt-icon" style="pointer-events: none; display: block; width: 100%; height: 100%;"><g class="style-scope yt-icon"><path d="M12,2C6.5,2,2,6.5,2,12c0,5.5,4.5,10,10,10s10-4.5,10-10C22,6.5,17.5,2,12,2z M9.8,17.3l-4.2-4.1L7,11.8l2.8,2.7L17,7.4 l1.4,1.4L9.8,17.3z" class="style-scope yt-icon"></path></g></svg>
                </div> 
              </div>
              <p class="text-sm text-gray-400">6,6 m Views</p>
              <p class="text-sm text-gray-400">59 minutes</p>
            </div>
           

          </div>
           <div class="flex flex-col px-2 pb-2 text-gray-400 hidden group-hover:block">
            <button class="w-full bg-gray-100 dark:bg-dark-100 flex items-center justify-center py-1 mb-2 ">
              <div class="w-8 h-8 p-1">
                <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false" class="style-scope yt-icon" style="pointer-events: none; display: block; width: 100%; height: 100%;"><g class="style-scope yt-icon"><path d="M14.97,16.95L10,13.87V7h2v5.76l4.03,2.49L14.97,16.95z M12,3c-4.96,0-9,4.04-9,9s4.04,9,9,9s9-4.04,9-9S16.96,3,12,3 M12,2c5.52,0,10,4.48,10,10s-4.48,10-10,10S2,17.52,2,12S6.48,2,12,2L12,2z" class="style-scope yt-icon"></path></g></svg>
              </div>
              <p>Watch Later</p>
            </button>
            <button class="w-full bg-gray-100 dark:bg-dark-100  flex items-center justify-center py-1 ">
              <div class="w-8 h-8 p-1">
                <svg viewBox="0 0 24 24" preserveAspectRatio="xMidYMid meet" focusable="false" class="style-scope yt-icon" style="pointer-events: none; display: block; width: 100%; height: 100%;"><g class="style-scope yt-icon"><path d="M21,16h-7v-1h7V16z M21,11H9v1h12V11z M21,7H3v1h18V7z M10,15l-7-4v8L10,15z" class="style-scope yt-icon"></path></g></svg>
              </div>
              <p>Add to Playlist</p>
            </button>
           </div>
        </div>
        </div>
        
      </div>
    </div>
  </div>
</template>

<style>
html, body, #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
 margin: 0;
 padding: 0;
}
</style>
