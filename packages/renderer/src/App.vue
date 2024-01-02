<script lang="ts" setup>
import {BeakerIcon} from '@heroicons/vue/24/solid';
import ReactiveCounter from '/@/components/ReactiveCounter.vue';
import BaseLayoutWithMenu from '/@/layouts/BaseLayoutWithMenu.vue';
</script>

<template>
  <BaseLayoutWithMenu title="Main App Title">
    <div class="m-10 p-10 text-center">
      <BeakerIcon class="h-36 w-36 text-lime-400 mx-auto my-4 drop-shadow-xl" />
      <h1 class="text-3xl mb-6">Electron Starter App</h1>
      <p>With Vue / Tailwind / Heroicons</p>
      <p>
        <ReactiveCounter />
      </p>
    </div>

    <p class="m-2 text-justify">
      Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint
      ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur
      officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor
      minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla
      sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia
      voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia
      eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris
      sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.
    </p>
    <p class="m-2 text-justify">
      Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint
      ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur
      officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor
      minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla
      sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia
      voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia
      eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris
      sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.
    </p>
    <p class="m-2 text-justify">
      Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint
      ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur
      officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor
      minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla
      sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia
      voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia
      eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris
      sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.
    </p>
  </BaseLayoutWithMenu>
</template>

<style lang="css"></style>
