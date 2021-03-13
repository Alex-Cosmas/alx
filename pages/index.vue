<template>
  <div>
    <div class="flex flex-col min-h-screen">
      <!-- Header Component -->
      <Header />
      <!--  -->

      <!-- Side bar + main body -->
      <div class="flex flex-1 ">
        <!-- SideBar Component -->
        <SideBar />

        <!-- Main Component -->
        <div class="w-full m-5">
          <!-- Main Components -->
          <MainComponent />
        </div>
      </div>
      <!-- End of side bar + main body -->
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
