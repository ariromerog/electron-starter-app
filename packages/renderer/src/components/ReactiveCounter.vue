<script lang="ts" setup>
import {ref} from 'vue';

const count = ref(0);
</script>

<template>
  <div class="m-3">
    <p> Test Component: </p>
    <button
      class="bg-lime-400 text-black p-3 rounded"
      @click="count++"
    >
      count is: {{ count }}
    </button>
  </div>
</template>
