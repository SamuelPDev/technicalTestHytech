<script setup>
import { NavMenu } from "../utils/data.js";
</script>

<template>
  <div class="flex flex-row">
    <div class="w-full">
      <header
        class="header sticky top-0 shadow-md flex items-center justify-between bg-[#0f0f0f] rounded-md"
      >
        <nav class="nav font-semibold text-sm">
          <ul class="flex items-center">
            <li
              :class="`p-4 border-b-2 border-green-500
               border-opacity-0 hover:border-opacity-100
               hover:text-green-500 duration-200 cursor-pointer active
               ${index === 0 && 'text-green-500 border-opacity-100  '}
               `"
              v-for="(item, index) in NavMenu"
            >
              <a :href="item.link">{{ item.text }}</a>
            </li>
          </ul>
        </nav>

        <div class="w-3/12 flex justify-end mr-2">
          <a href="#" class="p-0.5 hover:text-green-500 duration-200">
            <ion-icon name="save"></ion-icon>
          </a>
          <a href="#" class="p-0.5 hover:text-green-500 duration-200">
            <ion-icon name="create"></ion-icon>
          </a>
          <a href="#" class="p-0.5 hover:text-green-500 duration-200">
            <ion-icon name="trash"></ion-icon>
          </a>
        </div>
      </header>
    </div>
  </div>
</template>
