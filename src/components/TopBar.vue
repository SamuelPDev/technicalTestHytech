<script setup>
import { MenuItems } from "../utils/menu.js";
import Toggle from "./UI/Toggle.vue";
</script>

<template>
  <nav class="flex px-4 md:shadow-lg items-center relative bg-primary">
    <div
      class="flex flex-row items-center justify-between w-full text-lg font-bold md:py-0 py-4"
    >
      <div class="flex flex-row items-center">
        <div class="w-8 h-8 rounded-full bg-slate-700"></div>
        <div
          class="md:px-2 ml-auto md:flex md:space-x-2 absolute md:relative top-full left-0 right-0 font-semibold text-sm"
        >
          <ul class="flex items-center">
            <li v-for="items in MenuItems">
              <a href="#" class="flex md:inline-flex p-4 items-center">
                <ion-icon :name="items.icon"></ion-icon>
                <span class="ml-2 hover:text-green-500 duration-200">{{
                  items.text
                }}</span>
              </a>
            </li>
          </ul>
        </div>
      </div>

      <div class="flex flex-row items-center">
        <div
          class="flex flex-row items-center justify-center bg-gray-800 rounded-lg"
        >
          <div class="p-1 hover:text-green-500 duration-200">
            <ion-icon name="search-outline"></ion-icon>
          </div>
          <div class="p-1 hover:text-green-500 duration-200">
            <ion-icon name="scan-outline"></ion-icon>
          </div>
        </div>
        <div class="mx-5">
          <Toggle />
        </div>
        <div class="flex flex-row justify-between w-20 mx-2">
          <span class="hover:text-green-500 duration-200"
            ><ion-icon name="mail"></ion-icon
          ></span>
          <span class="hover:text-green-500 duration-200"
            ><ion-icon name="calendar"></ion-icon
          ></span>
          <span class="hover:text-green-500 duration-200"
            ><ion-icon name="notifications"></ion-icon
          ></span>
        </div>
        <div class="w-8 h-8 rounded-full bg-slate-700"></div>
      </div>
    </div>
  </nav>
</template>
