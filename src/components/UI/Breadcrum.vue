<script setup>
const breadcrum = ["Users", "Energy Efficiency", "Items 219"];
</script>

<template>
  <div class="flex flex-row items-center justify-center">
    <span
      v-for="(item, index) in breadcrum"
      class="flex flex-row items-center text-xs"
    >
      <span :class="index === breadcrum.length - 1 && 'text-green-400'">{{ item }}</span>
      <span>
        <ion-icon
          name="chevron-forward-outline"
          v-if="index < breadcrum.length - 1"
        ></ion-icon>
      </span>
    </span>
  </div>
</template>
