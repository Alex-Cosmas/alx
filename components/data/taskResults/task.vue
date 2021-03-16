<template>
  <div>
    <div class="px-6 mb-10">
      <div class="shadow-xl p-5">
        <div class="flex justify-between">
          <h5>{{ task.todo }}</h5>
          <div>
            <div class="bg-green-600 px-2 rounded text-white">
              <p>{{ task.type }}</p>
            </div>
          </div>
        </div>
        <p class="flex">
          Due date:
          <span class="px-2">{{ task.due }}</span>
        </p>
        <div class="flex items-center py-2">
          <div class="w-10 h-10 rounded-full bg-gray-900"></div>
          <p class="mx-4">{{ task.by }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import Contact from "~/components/data/contactResults/Contact";
// import ContactList from "~/components/data/contactResults/ContactList";
export default {
  props: {
    task: {
      type: Object,
      required: true
    }
  }
};
</script>
