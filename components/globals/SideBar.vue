<template>
  <div class="w-1/5 flex-none shadow-md bg-white">
    <div class="w-full px-8 my-5">
      <!-- Avatar -->
      <div class="mb-8 flex text-sm items-center font-semibold space-x-3">
        <img
          src="https://images.unsplash.com/photo-1557296387-5358ad7997bb?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=788&q=80"
          alt=""
          class="w-10 h-10 rounded-full object-cover"
        />
        <div class="leading-tight">
          <h2 class=" text-secondary-black">Sierra Ferguson</h2>
          <p class="font-xs font-normal tracking-tight text-accent-gray">
            s.ferguson@gmail.com
          </p>
        </div>
      </div>

      <ul class="flex flex-col space-y-4">
        <nuxt-link to="/" class="flex ">
          <div class="mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z"
              ></path>
            </svg>
          </div>
          Dashboard</nuxt-link
        >
        <nuxt-link to="/tasks" class="flex">
          <div class="mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 10V7m0 10a2 2 0 002 2h2a2 2 0 002-2V7a2 2 0 00-2-2h-2a2 2 0 00-2 2"
              ></path>
            </svg>
          </div>
          Tasks</nuxt-link
        >
        <nuxt-link to="" class="flex">
          <div class=" mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
              ></path>
            </svg>
          </div>
          Email</nuxt-link
        >
        <nuxt-link to="/contact" class="flex">
          <div class=" mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
              ></path>
            </svg>
          </div>
          Contacts</nuxt-link
        >
        <nuxt-link to="" class="flex">
          <div class=" mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"
              ></path>
            </svg>
          </div>
          Chat</nuxt-link
        >
        <nuxt-link to="" class="flex">
          <div class=" mr-2 text-main-blue">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 10V7m0 10a2 2 0 002 2h2a2 2 0 002-2V7a2 2 0 00-2-2h-2a2 2 0 00-2 2"
              ></path>
            </svg>
          </div>
          Deals</nuxt-link
        >
      </ul>
    </div>

    <hr class="border-gray-500" />
    <div class="w-full px-8 my-5 h-full">
      <div class="flex flex-col justify-between">
        <ul class="font-bold my-6 ">
          <li class="mb-3">Settings</li>
        </ul>

        <p>Toogle Sidebar</p>
      </div>
    </div>
  </div>
</template>
