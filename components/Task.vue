<template>
  <tbody>
    <tr class="bg-white">
      <td class="py-3 px-2">
        <label class="flex items-center">
          <input
            @click="$emit('delete-task', task.id)"
            type="checkbox"
            class="form-checkbox text-green-500"
          />
        </label>
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ task.status }}
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900">
        <div class="flex items-center ">
          {{ task.description }}
        </div>
      </td>

      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ task.assigned }}
      </td>

      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        <img
          :src="task.avatar"
          alt=""
          class="mr-2 h-6 w-6 bg-gray-900 rounded-full object-contain"
        />
      </td>
      <td class="py-4 whitespace-nowrap text-sm text-gray-500">
        {{ task.date }}
      </td>
    </tr>
  </tbody>
</template>

<script>
export default {
  name: "Task",
  props: {
    task: Object
  }
  // methods: {
  //   onDelete(id) {
  //     this.$emit("delete-task", id);
  //   }
  // }
};
</script>
