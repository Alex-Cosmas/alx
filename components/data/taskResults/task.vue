<template>
  <div>
    <div class="px-6 mb-10">
      <div class="py-3 px-5 shadow-xl">
        <div class="">
          <div class="flex justify-between ">
            <h5 class=" text-secondary-tableblack font-semibold">
              {{ task.todo }}
            </h5>
            <p class=" text-accent-gray">{{ task.type }}</p>
          </div>
          <div class="flex">
            Due Date:
            <p class="mx-4">{{ task.due }}</p>
          </div>
          <div class="flex justify-between items-center py-2">
            <div class="flex items-center ">
              <img
                src="https://images.unsplash.com/photo-1557296387-5358ad7997bb?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=788&q=80"
                alt=""
                class="w-6 h-6 rounded-full"
              />
              <p class="mx-4">{{ task.by }}</p>
            </div>
            <button class=" bg-main-green p-1 rounded-sm">Completed</button>
          </div>
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
