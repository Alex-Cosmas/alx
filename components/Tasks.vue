<template>
  <div>
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
                    Status
                  </th>

                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Description
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Assigned By
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Avatar
                  </th>
                  <th
                    scope="col"
                    class="py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Due Date
                  </th>
                </tr>
              </thead>

              <Task
                v-for="task in tasks"
                :key="task.id"
                v-on:delete-task="$emit('delete-task', task.id)"
                :task="task"
              />

              <!--  -->
            </table>
          </div>
        </div>
      </div>
    </div>
    <!--  -->
  </div>
</template>

<script>
import Task from "~/components/Task";
export default {
  name: "Tasks",
  props: {
    tasks: Array
  },
  components: {
    Task
  },
  emits: ["delete-task"]
};
</script>
