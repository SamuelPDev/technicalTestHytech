<script setup>
import { SideMenu } from "../utils/menu.js";
</script>

<template>
  <div class="w-full flex items-center justify-center">
    <div class="bg-[#0f0f0f] w-10/12 min-h-full mt-5">
      <div class="w-full h-32 bg-gray-800">
        <div class="relative w-full h-full">
          <div
            class="absolute -bottom-5 left-5 w-20 h-20 rounded-full bg-slate-700"
          ></div>
        </div>
      </div>
      <div class="flex flex-col mt-5 p-3">
        <span>Testing_possible_username_length</span>
        <span class="text-green-400 text-xs"
          >Testing_possible_username_length</span
        >
      </div>
      <div class="mt-5">
        <div>
          <ul class="flex items-center text-xs">
            <li
              :class="`p-4 border-b-2 border-green-500
                border-opacity-0 hover:border-opacity-100 
                hover:text-green-500 duration-200 cursor-pointer
                ${index === 0 && 'text-green-500 border-opacity-100  '}
                `"
              v-for="(item, index) in SideMenu"
            >
              <span class="mr-2">
                <ion-icon :name="item.icon"></ion-icon>
              </span>
              <span>{{ item.text }}</span>
            </li>
          </ul>
        </div>
      </div>
      <div class="flex flex-col">
        <div class="flex flex-row justify-between items-center w-full p-5">
          <span>Main Contact</span>
          <ion-icon name="swap-vertical-outline"></ion-icon>
        </div>
        <div class="w-full flex items-center justify-center">
          <div class="flex flex-col w-11/12 bg-gray-900 text-xs p-2">
            <div class="flex flex-row w-10/12 justify-between">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">First Name</span>
                <span>Pearline</span>
              </div>
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Last Name</span>
                <span>Hodkiewicz</span>
              </div>
            </div>
            <div class="flex flex-row w-full justify-between my-3">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Email</span>
                <span>Pearline56@hotmail.com</span>
              </div>
            </div>
            <div class="flex flex-row w-10/12 justify-between">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Mobile Phone</span>
                <span>934-879-9187</span>
              </div>
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Home Phone</span>
                <span>486-542-1541</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="flex flex-col my-5">
        <div class="flex flex-row justify-between items-center w-full p-5">
          <span>Main Propierty</span>
          <ion-icon name="swap-vertical-outline"></ion-icon>
        </div>
        <div class="w-full flex items-center justify-center">
          <div class="flex flex-col w-11/12 bg-gray-900 text-xs p-2">
            <div class="flex flex-row w-10/12 justify-between">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">State</span>
                <span>Minnesota</span>
              </div>
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">City</span>
                <span>North Ayana</span>
              </div>
            </div>
            <div class="flex flex-row w-full justify-between my-3">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Street Adress</span>
                <span>50078 Kristin Junction</span>
              </div>
            </div>
            <div class="flex flex-row w-10/12 justify-between">
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Apt</span>
                <span>Apt 158</span>
              </div>
              <div class="flex flex-col">
                <span class="text-gray-600 text-xs mb-1">Home Phone</span>
                <span>80860-5560</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
