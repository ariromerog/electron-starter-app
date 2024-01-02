<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
defineProps(['title']);
</script>

<template>
  <div class="header bg-stone-900 text-gray-200 p-2 shadow-md">
    <h1>
      <BeakerIcon class="h-6 w-6 text-lime-500 float-left mx-2" />
      {{ title }}
    </h1>
  </div>
  <div class="menu">
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
  </div>
  <div class="content">
    <slot />
  </div>
</template>

<style lang="css">
.header {
  position: fixed;
  z-index: 100;
  top: 0;
  left: 0;
  right: 0;
  height: 40px;
}
.content {
  padding: 60px 20px 20px 60px;
}
.menu {
  position: fixed;
  background: #444;
  z-index: 10;
  top: 40px;
  left: 0;
  width: 40px;
  bottom: 0;
  overflow-y: auto;
}
</style>
