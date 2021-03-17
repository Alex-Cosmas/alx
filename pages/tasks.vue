<template>
  <div>
    <div class="flex flex-col sm:flex-row min-h-screen overflow-x-hidden">
      <!-- Header Component -->

      <!--  -->
      <!-- Side bar + main body -->
      <div class="flex flex-1 ">
        <!-- SideBar Component -->
        <SideBar />
        <!-- Main Component -->

        <div class="w-full">
          <!-- Start of Search Component -->
          <div
            class="bg-white flex-grow flex justify-between pr-12 py-5 shadow-md h-16"
          >
            <div class="px-6 flex items-center w-full">
              <svg
                class="w-5 h-5 text-accent-icongray"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                />
              </svg>
              <input
                type="text"
                placeholder="Global Search"
                name=""
                id=""
                class="w-full text-sm pl-3"
              />
            </div>
            <svg
              class="w-5 h-5 text-accent-icongray"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                strokeLinecap="round"
                strokeLinejoin="round"
                strokeWidth="{2}"
                d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
              />
            </svg>
          </div>
          <!-- End of Search Component -->
          <div class="m-5">
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
      </div>
      <!-- End of side bar + Main body -->
    </div>
  </div>
</template>
<script>
import SideBar from "~/components/globals/SideBar";
import Button from "~/components/elements/Button";
import MyTasks from "~/components/Tasks";

export default {
  components: {
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
