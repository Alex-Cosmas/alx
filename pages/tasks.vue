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
          <!--  -->
          <div class="flex items-center justify-between my-8">
            <p>Status: <span>All</span></p>
            <!-- <button
              class="bg-blue-500 text-white rounded-md shadow-sm px-8 py-2"
            >
              Add contact
            </button> -->
            <Button text="Add Tasks" />
          </div>
          <MyTasks :tasks="tasks" />
          <!--  -->
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
import Button from "~/components/elements/Button";
import MyTasks from "~/components/Tasks";

export default {
  components: {
    Header,
    SideBar,
    Button,
    MyTasks
  },
  data() {
    return {
      tasks: []
    };
  },
  created() {
    this.tasks = [
      {
        id: 1,
        description: "Send benefit review by Sunday",
        date: "December 23, 2020",
        status: "Reminder",
        assigned: "George Fields",
        avatar:
          "https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png"
      },
      {
        id: 2,
        description: "Invite to office meet-up",
        date: "December 23, 2020",
        status: "Ended",
        assigned: "Lindsey Stroud",
        avatar:
          "https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png"
      },
      {
        id: 3,
        description: "Office meet-up",
        date: "December 23, 2020",
        status: "Completed",
        assigned: "Nicci Troiani",
        avatar:
          "https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png"
      }
    ];
  }
};
</script>
