<script setup>
const props = defineProps({
  checkboxesData: Object,
});
</script>
<template>
  <div class="flex flex-col space-y-1.5">
    <div
      v-for="(item, index) in checkboxesData"
      :key="index"
      class="flex space-x-2 items-center"
    >
      <input
        type="checkbox"
        :name="item.name"
        :id="`checkbox${index}`"
        class="form-checkbox"
      />
      <label :for="`checkbox${index}`" class="text-sm font-small">{{
        item.text
      }}</label>
    </div>
  </div>
</template>
