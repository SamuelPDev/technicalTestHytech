<script setup>
import Breadcrum from "./UI/Breadcrum.vue";
</script>

<template>
  <div class="w-full flex flex-row justify-between bg-[#0f0f0f] p-1">
    <div class="flex flex-row items-center">
      <div
        class="flex flex-row items-center justify-center bg-gray-800 rounded-lg mr-5"
      >
        <div class="p-[2px] hover:text-green-500 duration-200">
          <ion-icon name="arrow-back-outline"></ion-icon>
        </div>
        <div class="p-[2px] hover:text-green-500 duration-200">
          <ion-icon name="arrow-forward-outline"></ion-icon>
        </div>
      </div>
      <Breadcrum />
    </div>
    <div class="flex flex-row items-center mx-2 rounded-lg">
      <div
        class="p-[2px] mr-2 hover:text-green-500 duration-200 bg-gray-700 rounded-lg"
      >
        <ion-icon name="eye-outline"></ion-icon>
      </div>
      <div
        class="p-[2px] mr-2 hover:text-green-500 duration-200 bg-gray-700 rounded-lg"
      >
        <ion-icon name="repeat-outline"></ion-icon>
      </div>

      <div class="p-[2px] bg-gray-700 mr-2 rounded-lg">
        <span class="hover:text-green-500 duration-200">
          <ion-icon name="add-outline"></ion-icon>
        </span>

        <span class="mx-2 hover:text-green-500 duration-200">
          <ion-icon name="create-outline"></ion-icon>
        </span>
        <span class="hover:text-green-500 duration-200">
          <ion-icon name="trash-outline"></ion-icon>
        </span>
      </div>

      <div
        class="p-[2px] bg-gray-700 mr-2 hover:text-green-500 duration-200 rounded-lg"
      >
        <ion-icon name="ellipsis-vertical-outline"></ion-icon>
      </div>
    </div>
  </div>
</template>
