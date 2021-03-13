<template>
  <div class="flex">
    <!--  Fist  Half -->
    <div class="bg-white rounded-lg shadow-sm flex-grow h-screen">
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
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              24
            </div>
          </div>
          <div class="flex flex-col">
            Tue
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              25
            </div>
          </div>
          <div class="flex flex-col">
            Wed
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              26
            </div>
          </div>
          <div class="flex flex-col">
            Thu
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              27
            </div>
          </div>
          <div class="flex flex-col">
            Fri
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              28
            </div>
          </div>
          <div class="flex flex-col">
            Sat
            <div class="w-8 h-8 rounded-full flex items-center justify-center">
              29
            </div>
          </div>
        </div>
      </div>
      <div class="px-6 mb-10">
        <div class="shadow-xl p-5">
          <div class="flex justify-between">
            <h5>Send benefit review by Sunday</h5>
            <div>
              <div class="bg-green-600 px-2 rounded text-white">
                <p>Reminder</p>
              </div>
            </div>
          </div>
          <p class="flex">
            Due date:
            <span class="px-2">December 23, 2020</span>
          </p>
          <div class="flex items-center py-2">
            <div class="w-10 h-10 rounded-full bg-gray-900"></div>
            <p class="mx-4">George Fields</p>
          </div>
        </div>
      </div>
    </div>

    <!--  Second Half -->
    <div class="w-1/2 flex flex-col justify-between ml-8">
      <div class="h-full bg-white rounded p-3 mb-3">
        Deals
      </div>
      <div class="h-full  bg-white rounded p-3">
        Tasks
      </div>
    </div>
    <!--  Second Half -->
  </div>
</template>
