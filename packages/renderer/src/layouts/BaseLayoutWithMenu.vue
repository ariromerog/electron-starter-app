<script lang="ts" setup>
import {ref} from 'vue';
import {CommandLineIcon} from '@heroicons/vue/24/solid';
defineProps(['title']);
const isActive = ref(false);

function toggleMenu(): void {
  isActive.value = !isActive.value;
}
</script>

<template>
  <div
    id="header"
    class="bg-gradient-to-r from-zinc-900 to-zinc-800 text-gray-200 p-2 shadow-md"
  >
    <h1>
      <CommandLineIcon
        class="h-6 w-6 text-lime-500 float-left mr-4 cursor-pointer"
        @click="toggleMenu"
      />
      {{ title }}
    </h1>
  </div>
  <div
    id="menu"
    :class="{active: isActive}"
    class="bg-zinc-800"
  >
    <div>
      <button class="bg-zinc-700"> 1 </button>
    </div>
    <div>
      <button class="bg-zinc-700"> 1 </button>
    </div>
    <div>
      <button class="bg-zinc-700"> 1 </button>
    </div>
  </div>
  <div
    id="content"
    class="bg-zinc-800"
  >
    <slot />
  </div>

  <div
    id="footer"
    class="bg-lime-600 text-center text-white text-sm"
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
  left: 50px;
  right: 0;
  bottom: 20px;
  overflow: auto;
}

#menu {
  position: absolute;
  top: 40px;
  left: 0;
  bottom: 20px;
  width: 49px;
  overflow-y: auto;
  overflow-x: hidden;
  z-index: 100;
  transition: 0.3s ease-in width;
}
#menu.active {
  width: 300px;
  transition: 0.3s ease-out width;
}

#footer {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 20px;
}

#menu button {
  margin: 10px;
  padding: 4px;
  width: 30px;
  text-align: center;
  border-radius: 4px;
  cursor: pointer;
}
</style>
