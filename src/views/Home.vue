<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>m3u8 Downloader</h1>
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
