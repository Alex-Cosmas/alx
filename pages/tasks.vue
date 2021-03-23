<template>
  <div>
    <div class="flex flex-col sm:flex-row min-h-screen overflow-x-hidden">
      <div class=" bg-secondary-tableblack text-white sm:w-1/4">
        <SideBar />
      </div>
      <div class=" w-full block">
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
            <!-- Top Bar -->
            <div
              class="flex items-center justify-between my-8"
              @toggle-add-task="toggleAddTask"
            >
              <p>Status: <span>All</span></p>

              <Button
                @toggle-add-task="$emit('toggle-add')"
                text="Add Tasks"
                class=" bg-main-blue"
              />
            </div>

            <!-- Add Task Component -->
            <div v-show="showAddTask">
              <AddTask @add-task="addTask" />
            </div>
            <!-- End -->

            <MyTasks @delete-task="deleteTask" :tasks="tasks" />

            <!--  -->
          </div>
          <!--  -->
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import SideBar from '~/components/globals/SideBar';
import Button from '~/components/elements/Button';
import MyTasks from '~/components/Tasks';

import AddTask from '~/components/AddTask';
export default {
  components: {
    SideBar,
    Button,
    MyTasks,
    AddTask
  },
  data() {
    return {
      tasks: [],
      showAddTask: false
    };
  },
  methods: {
    toggleAddTask() {
      this.showAddTask = !this.showAddTask;
    },
    addTask(task) {
      this.tasks = [...this.tasks, task];
    },
    deleteTask(id) {
      // console.log("task", id);

      this.tasks = this.tasks.filter(task => task.id !== id);
    }
  },

  created() {
    this.tasks = [
      {
        id: 1,
        description: 'Send benefit review by Sunday',
        date: 'December 23, 2020',
        status: 'Reminder',
        assigned: 'George Fields',
        avatar:
          'https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png'
      },
      {
        id: 2,
        description: 'Invite to office meet-up',
        date: 'December 23, 2020',
        status: 'Ended',
        assigned: 'Lindsey Stroud',
        avatar:
          'https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png'
      },
      {
        id: 3,
        description: 'Office meet-up',
        date: 'December 23, 2020',
        status: 'Completed',
        assigned: 'Nicci Troiani',
        avatar:
          'https://thumbnailer.mixcloud.com/unsafe/42x42/defaults/users/1.png'
      }
    ];
  }
};
</script>
