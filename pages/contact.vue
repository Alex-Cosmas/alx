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
          <!-- Contact Component -->
          <Contacts />
          <!-- End of Contact Component -->
        </div>
        <!--  -->
      </div>
      <!-- End of side bar + Main body -->
    </div>
  </div>
</template>

<script>
import Header from "~/components/globals/Header";
import SideBar from "~/components/globals/SideBar";
import Contacts from "~/components/data/Contacts";

export default {
  components: {
    Header,
    SideBar,
    Contacts
  }
};
</script>
