<script setup>
import { FormPersonalDetails, Checkboxes } from "../utils/data.js";
import CheckboxGroup from "./UI/CheckboxGroup.vue";
import AmountInput from "./UI/AmountInput.vue";
import Toggle from "./UI/Toggle.vue";
</script>
<template>
  <div class="flex items-center justify-center bg-[#0f0f0f] mt-5 rounded-md">
    <div class="mx-auto w-full">
      <div class="flex justify-between items-center py-4 px-2">
        <label for="label1" class="text-lg font-medium">Personal Details</label>
        <Toggle />
      </div>
      <form action="" method="POST">
        <div class="-mx-3 grid grid-cols-3 gap-4 w-full px-12">
          <div v-for="item in FormPersonalDetails">
            <div class="mb-5 text-white">
              <label for="label1" class="block text-sm font-medium pb-2">{{
                item.label
              }}</label>
              <div
                class="flex flex-row px-2 items-center bg-gray-800 rounded-md"
              >
                <span class="rounded-l-lg px-1">
                  <ion-icon name="ellipsis-horizontal-outline"></ion-icon>
                </span>
                <input
                  type="text"
                  :name="item.name"
                  id="label"
                  :placeholder="item.placeholder"
                  class="w-full border border-gray-800 bg-gray-800 py-2 px-4 text-sm font-medium text-white outline-none focus:shadow-md"
                />
                <span class="py-2">
                  <ion-icon name="pencil" class="text-white"></ion-icon>
                </span>
              </div>
            </div>
          </div>
          <div>
            <label for="label1" class="block text-sm font-medium pb-2">
              Label
            </label>
            <CheckboxGroup :checkboxesData="Checkboxes" />
          </div>
          <div>
            <label for="label1" class="block text-sm font-medium pb-2">
              Channel Partner
            </label>
            <AmountInput />
          </div>
          <div>
            <label for="label1" class="block text-sm font-medium pb-2">
              Channel Partner
            </label>
            <AmountInput />
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
