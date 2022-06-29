<template>
    <div class="fixed right-0 z-10 pl-20 w-full bg-white dark:bg-dark-600 dark:border-dark-100 border-b">
        <div></div>
        <div class="p-2 flex">
            <button v-for="topic, index in topics" :key="topic" :class="` text-sm mr-2 px-3 hover:bg-gray-200 ${(index ==0)?'bg-black dark:bg-gray-100 dark:text-dark-600 text-white':' border bg-gray-100 text-gray-800 dark:bg-dark-300 dark:border-dark-100 dark:text-white'}  rounded-full flex`">
                <p>{{topic}}</p>
            </button>
        </div>
        <div></div>
    </div>
</template>

<script lang="ts">
    export default{
        data(){
            return{
                topics:[
                    "All",
                    "Games",
                    "Blender",
                    "Computer Software",
                    "DC Comics"
                ]
            }
        }
    }
</script>