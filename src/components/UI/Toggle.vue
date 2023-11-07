<script setup>
import { ref } from "vue";

const toggleInput = ref();
</script>

<template>
  <div>
    <div
      class="relative inline-block w-10 mr-2 align-middle select-none transition duration-200 ease-in"
    >
      <input
        type="checkbox"
        name="toggle"
        id="toggle"
        v-model="toggleInput"
        :class="`toggle-checkbox absolute block
        w-6 h-6 rounded-full bg-green-600 border-4
        appearance-none cursor-pointer
        ${toggleInput && 'right-0 border-green-400 bg-green-400'}
        `"
      />
      <label
        for="toggle"
        class="toggle-label block overflow-hidden h-6 rounded-full bg-gray-800 cursor-pointer"
      >
      </label>
    </div>
  </div>
</template>
