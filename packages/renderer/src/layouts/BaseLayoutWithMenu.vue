<script lang="ts" setup>
import {AcademicCapIcon, BeakerIcon, BuildingOffice2Icon} from '@heroicons/vue/24/solid';
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
  <div
    id="menu"
    class="from-stone-800 to-stone-900 bg-gradient-to-r"
  >
    <BeakerIcon class="h-10 w-10 text-stone-400 m-4" />
    <BuildingOffice2Icon class="h-10 w-10 text-stone-400 m-4" />
    <AcademicCapIcon class="h-10 w-10 text-stone-400 m-4" />
    <BeakerIcon class="h-10 w-10 text-stone-400 m-4" />
    <BuildingOffice2Icon class="h-10 w-10 text-stone-400 m-4" />
    <AcademicCapIcon class="h-10 w-10 text-stone-400 m-4" />
    <BeakerIcon class="h-10 w-10 text-stone-400 m-4" />
    <BuildingOffice2Icon class="h-10 w-10 text-stone-400 m-4" />
    <AcademicCapIcon class="h-10 w-10 text-stone-400 m-4" />
    <BeakerIcon class="h-10 w-10 text-stone-400 m-4" />
    <BuildingOffice2Icon class="h-10 w-10 text-stone-400 m-4" />
    <AcademicCapIcon class="h-10 w-10 text-stone-400 m-4" />
  </div>
  <div id="content">
    <slot />
  </div>

  <div
    id="footer"
    class="bg-stone-600 text-center text-sm"
  >
    footer
  </div>
</template>

<style lang="css">
#header {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 40px;
  z-index: 1000;
  overflow: hidden;
}

#content {
  position: absolute;
  top: 40px;
  left: 100px;
  right: 0;
  bottom: 20px;
  overflow: auto;
}

#menu {
  position: absolute;
  top: 40px;
  left: 0;
  bottom: 20px;
  width: 100px;
  overflow: auto;
  z-index: 100;
}

#footer {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 20px;
}
</style>
