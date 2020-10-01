<template>
  <div class="bg-gray-100">
    <div class="container m-auto">
      <div class="flex flex-col justify-center items-center h-screen">
        <h1 class="text-3xl text-green-500 font-semibold">.m3u8 Downloader</h1>
        <div class="my-4 w-full flex justify-center">
          <input class="border border-grey-300 focus:border-green-500 border-solid outline-none w-6/12 py-2 px-3 rounded" placeholder="Please input .m3u8 link here" type="text">
        </div>
        <button class="border border-green-500 py-2 px-3 bg-green-500 text-white rounded">
          <i class="fas fa-file-download mr-2"></i>
          Download
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import { useRoute, useRouter } from 'vue-router'; // @ is an alias to /src

export default defineComponent({
  name: 'Home',
  setup (props, ctx) {
    const route = useRoute()
    const router = useRouter()

    console.log(route.fullPath)

  }
});
</script>
