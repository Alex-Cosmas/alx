<template>
  <div>
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
    <div>
      <div class="flex flex-col sm:flex sm:flex-row m-5 min-h-screen">
        <!--  Fist  Half -->
        <div class="bg-white rounded-lg shadow-sm flex-grow h-auto">
          <div class="p-6 ">
            <div class="mb-3 flex justify-between">
              <p>8 tasks completed out of 10</p>
              <div>
                <p>
                  Show:
                  <span class=" text-blue-500">This Week</span>
                </p>
              </div>
            </div>
            <div class="bg-gray-200 p-1">
              <div class="bg-green-400 w-5/6 p-1"></div>
            </div>
          </div>
          <div class="px-6 mb-10 font-semibold">
            23 December, Sunday
          </div>
          <div class="px-6 mb-10">
            <div class="flex justify-between">
              <div class="flex flex-col">
                Sun
                <div
                  class="bg-blue-500 w-8 h-8 rounded-full text-white flex items-center justify-center "
                >
                  23
                </div>
              </div>
              <div class="flex flex-col">
                Mon
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  24
                </div>
              </div>
              <div class="flex flex-col">
                Tue
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  25
                </div>
              </div>
              <div class="flex flex-col">
                Wed
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  26
                </div>
              </div>
              <div class="flex flex-col">
                Thu
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  27
                </div>
              </div>
              <div class="flex flex-col">
                Fri
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  28
                </div>
              </div>
              <div class="flex flex-col">
                Sat
                <div
                  class="w-8 h-8 rounded-full flex items-center justify-center"
                >
                  29
                </div>
              </div>
            </div>
          </div>

          <TaskList :tasks="tasks" />

          <!--  -->
        </div>

        <!--  Second Half -->
        <div
          class="sm:w-1/2 flex flex-col justify-between sm:ml-8 my-10 sm:my-0"
        >
          <div class="h-full bg-white rounded p-3 mb-3">
            Deals
          </div>
          <div class="h-full  bg-white rounded p-3">
            Tasks
          </div>
        </div>
        <!--  Second Half -->
      </div>
    </div>
  </div>
</template>

<script>
import TaskList from "~/components/data/taskResults/taskList";
//
import data from "~/src/tasks.json";
//

export default {
  components: {
    TaskList
  },
  data() {
    return {
      tasks: data.tasks
    };
  }
};
</script>
