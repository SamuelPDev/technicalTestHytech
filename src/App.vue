<script setup>
import FormPropertiesDetails from "./components/FormPropertiesDetails.vue"
import FormPersonalDetails from "./components/FormPersonalDetails.vue";
import NavigationBar from "./components/NavigationBar.vue";
import Stepline from "./components/UI/StepLine.vue";
import OptionBar from "./components/OptionBar.vue"
import SideBar from "./components/SideBar.vue";
import MenuBar from "./components/MenuBar.vue"
import TopBar from "./components/TopBar.vue";

</script>

<template>

  <TopBar />
  <NavigationBar />
  <div class="flex flex-row ml-5">
    <div class="flex flex-col w-9/12 pb-8">
      <Stepline />
      <MenuBar />
      <OptionBar />
      <FormPersonalDetails />
      <FormPropertiesDetails />
    </div>
    <div class="w-3/12">
      <SideBar />
    </div>
  </div>
</template>

