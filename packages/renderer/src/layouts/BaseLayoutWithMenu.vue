<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
defineProps(['title']);
</script>

<template>
  <div
    id="header"
    class="bg-stone-900 text-gray-200 p-2 shadow-md"
  >
    <h1>
      <BeakerIcon class="h-6 w-6 text-lime-500 float-left mx-2" />
      {{ title }}
    </h1>
  </div>
  <div id="menu">
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
    <BeakerIcon class="h-6 w-3 text-stone-400 mx-auto my-4 drop-shadow-xl" />
  </div>
  <div id="content">
    <slot />
  </div>
</template>

<style lang="css">
#header {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 40px;
}

#content {
  position: absolute;
  top: 50px;
  left: 100px;
  right: 0;
  bottom: 30px;
  overflow: auto;
}

#menu {
  position: absolute;
  top: 50px;
  left: 0;
  bottom: 30px;
  width: 90px;
  overflow: auto;
}
</style>
