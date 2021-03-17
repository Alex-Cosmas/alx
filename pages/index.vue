<template>
  <div>
    <div>
      <div class="flex flex-col sm:flex-row min-h-screen overflow-x-hidden">
        <div class=" bg-secondary-tableblack text-white sm:w-1/5">
          <SideBar />
        </div>
        <div class=" w-full block">
          <MainComponent />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "~/components/globals/Header";
import SideBar from "~/components/globals/SideBar";
import MainComponent from "~/components/globals/MainComponent";

export default {
  components: {
    Header,
    SideBar,
    MainComponent
  }
};
</script>
