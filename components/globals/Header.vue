<template>
  <!-- Header -->
  <div class="bg-white flex items-center">
    <div class="w-1/5 flex-none">
      <div class="py-5 shadow-md">
        <nuxt-link to="/">
          <h6 class="shadow-2xl font-bold px-8 text-main-blue">Saas Kit</h6>
        </nuxt-link>
      </div>
    </div>

    <div class="flex-grow flex justify-between pr-12">
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
  </div>
  <!-- End of Header -->
</template>
