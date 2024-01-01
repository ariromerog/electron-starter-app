<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
defineProps(['title']);
</script>

<template>
  <div class="main-container">
    <div class="header bg-gray-800 p-2 shadow-xl">
      <h1>
        <BeakerIcon class="h-6 w-6 text-lime-500 float-left mx-2" />
        {{ title }}
      </h1>
    </div>
    <div class="content">
      <slot />
    </div>
    <hr />
  </div>
</template>

<style lang="css">
.main-container {
  height: 100vh;
  display: flex;
  flex-direction: column;
}
.header {
}

.content {
  height: 100%;
  overflow: auto;
}
</style>
