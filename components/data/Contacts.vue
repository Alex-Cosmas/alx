<template>
  <div>
    <!--  -->
    <div>
      <p>Company: <span>All</span></p>
    </div>
    <!--  -->
    <div class="flex flex-col">
      <div class="-my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
        <div class="py-2 align-middle inline-block min-w-full sm:px-6 lg:px-8">
          <div
            class="shadow overflow-hidden border-b border-gray-200 sm:rounded-lg"
          >
            <table class="min-w-full divide-y divide-gray-200">
              <thead class="bg-white">
                <tr>
                  <th scope="col" class="py-3 px-2">
                    <label class="inline-flex items-center">
                      <input
                        type="checkbox"
                        class="form-checkbox text-green-500"
                      />
                    </label>
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Name
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Email
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Company Name
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Role
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Forecast
                  </th>
                  <th
                    scope="col"
                    class="py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Recent Activity
                  </th>
                </tr>
              </thead>
              <tbody>
                <tr class="bg-white">
                  <td class="py-3 px-2">
                    <label class="flex items-center">
                      <input
                        type="checkbox"
                        class="form-checkbox text-green-500"
                      />
                    </label>
                  </td>
                  <td
                    class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900"
                  >
                    <div class="flex items-center ">
                      <img
                        src="https://images.unsplash.com/photo-1557296387-5358ad7997bb?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=788&q=80"
                        alt=""
                        class="mr-2 h-6 w-6 bg-gray-900 rounded-full object-contain"
                      />
                      Lindsey Stroud
                    </div>
                  </td>
                  <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                    lindsey.stroud@gmail.com
                  </td>
                  <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                    Hatchbuck
                  </td>
                  <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                    Manager
                  </td>
                  <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                    50 %
                  </td>
                  <td class="py-4 whitespace-nowrap text-sm text-gray-500">
                    5 Minutes ago
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
    <!--  -->
  </div>
</template>
