<template>
  <tbody>
    <tr class="bg-white">
      <td class="py-3 px-2">
        <label class="flex items-center">
          <input type="checkbox" class="form-checkbox text-green-500" />
        </label>
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900">
        <div class="flex items-center ">
          <img
            :src="contact.avatar"
            alt=""
            class="mr-2 h-6 w-6 bg-gray-900 rounded-full object-contain"
          />
          {{ contact.name }}
        </div>
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ contact.email }}
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ contact.company }}
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ contact.role }}
      </td>
      <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
        {{ contact.forecast }}
      </td>
      <td class="py-4 whitespace-nowrap text-sm text-gray-500">
        {{ contact.activity }}
      </td>
    </tr>
  </tbody>

  <!--  -->
</template>

<script>
export default {
  props: {
    contact: {
      type: Object,
      required: true
    }
  }
};
</script>
