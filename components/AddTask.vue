<template>
  <div>
    <form @submit="onSubmit" class="w-full space-y-6 p-6 shadow-md">
      <div class="flex flex-col block">
        <label class="">Task</label>
        <input
          v-model="text"
          type="text"
          name="text"
          placeholder="Add Task"
          class="px-3 py-2 border-b-2 focus:outline -none focus:bg-gray-100 focus:text-red-500"
        />
      </div>

      <div class="flex flex-col  block form-control">
        <label for="">Day & Time</label>
        <input
          v-model="day"
          type="text"
          name="day"
          placeholder="Add Day & Time"
          class="px-3 py-2 border-b-2 focus:outline -none focus:bg-gray-100 focus:text-red-500"
        />
      </div>

      <div class="form-control">
        <label for="">Set Reminder</label>
        <input
          v-model="reminder"
          type="checkbox"
          name="reminder"
          class="px-3 py-2 border-b-2 focus:outline -none focus:bg-gray-100 focus:text-red-500"
        />
      </div>

      <div v-if="!image">
        <h2>Select an image</h2>
        <input type="file" @change="onFileChange" />
      </div>
      <div v-else>
        <img :src="image" />
        <button @click="removeImage">Remove image</button>
      </div>

      <input
        type="submit"
        value="Save Task"
        class="w-full bg-gray-900 text-white border border-red-500 px-4 py-2 transition duration-50 focus:outline-none font-semibold hover:bg-red-500 hover:text-white text-xl cursor-pointer"
      />
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      image: '',
      text: '',
      day: '',
      reminder: false
    };
  },
  methods: {
    onSubmit(e) {
      e.preventDefault();

      if (!this.text) {
        alert("Please add a task");
        return;
      }

      const newTask = {
        id: Math.floor(Math.random() * 100000),
        text: this.text,
        day: this.day,
        reminder: this.reminder
      };

      this.$emit("add-task", newTask);

      this.text = '' ,
      this.day = '', 
      this.reminder = false


      
    },
    onFileChange(e) {
      var files = e.target.files || e.dataTransfer.files;
      if (!files.length) return;
      this.createImage(files[0]);
    },
    createImage(file) {
      var image = new Image();
      var reader = new FileReader();
      var vm = this;

      reader.onload = e => {
        vm.image = e.target.result;
      };
      reader.readAsDataURL(file);
    },
    removeImage: function(e) {
      this.image = '';
    }
  }
};
</script>

<style scoped>
img {
  width: 5%;
  margin: auto;
  display: block;
  margin-bottom: 10px;
}
</style>
