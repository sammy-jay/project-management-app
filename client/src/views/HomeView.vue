<script setup>
import { reactive } from 'vue'

const state = reactive({ count: 0 })

function increment() {
  state.count++
}
</script>

<template>
    <div class="bg-gray-300 p-3 mx-auto mt-5 rounded-md shadow-md w-[150px] flex flex-col items-center">
        <p class="font-semibold text-5xl text-center">{{state.count}}</p>
        <button class="rounded-full px-3 py-1 bg-green-400 text-grey-300 cursor-pointer mt-5 w-[90%]" @click="increment()">increment</button>
    </div>

</template>
