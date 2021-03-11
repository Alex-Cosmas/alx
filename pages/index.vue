<template>
  <div>
    <!-- Header -->
    <div class="bg-white flex px-12 items-center">
      <div class="border-r-2 border-gray-200 w-48 py-5">
        <h6 class="shadow-2xl font-bold">Saas Kit</h6>
      </div>
      <div class="flex-grow flex justify-between pr-12">
        <div class="px-6">
          Global Search
        </div>
        Notification
      </div>
    </div>

    <!-- Side Menu + Main Div -->

    <div class="flex p-12">
      <div class=" w-48">
        <div class="flex h-screen">
          <div class="border-r border-gray-200 w-64">
            <h6 class="font-bold mb-4">Home</h6>
            <ul>
              <li class="mb-3">Dashboard</li>
              <li class="mb-3">Task</li>
              <li class="mb-3">Email</li>
              <li class="mb-3">Chat</li>
              <li class="mb-3">Deals</li>
            </ul>

            <ul class="font-bold my-6">
              <li class="mb-3">Settings</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="flex-grow px-6">
        <div>
          <!-- Grid Columns -->
          <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <p>Col-6</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-sm">
              <p>Col-6</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>
