<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
defineProps(['title']);
</script>

<template>
  <div class="main-container">
    <div class="header bg-stone-900 text-gray-200 p-2 shadow-md">
      <h1>
        <BeakerIcon class="h-6 w-6 text-lime-500 float-left mx-2" />
        {{ title }}
      </h1>
    </div>
    <div class="content bg-stone-800 text-gray-50">
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

.content {
  height: 100%;
  overflow: auto;
}
</style>
