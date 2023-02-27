<template>
  <div>
    <button @click="handle(1)">click me</button>
  </div>
</template>

<script setup name="Explore">
import router from "@/router";


const route = useRoute();
const { proxy } = getCurrentInstance();

function handle(storyId) {
  router.push({ path: "/eboard/story/index/" + storyId});
}
</script>

<style scoped>

</style>