<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
import ReactiveCounter from '/@/components/ReactiveCounter.vue';
</script>

<template>
  <div class="m-10 p-10 text-center">
    <BeakerIcon class="h-36 w-36 text-lime-400 mx-auto my-4" />
    <h1 class="text-3xl mb-6">Electron Starter App</h1>
    <p>With Vue / Tailwind / Heroicons</p>
    <p>
      <ReactiveCounter />
    </p>
  </div>
</template>
