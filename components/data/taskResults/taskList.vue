<template>
  <div>
    <!-- TaskList -->
    <Task v-for="(task, index) in tasks" :key="index" :task="task" />
  </div>
</template>
<script>
import Task from "~/components/data/taskResults/task";

export default {
  props: {
    tasks: {
      type: Array,
      required: true
    }
  },
  components: {
    Task
  }
};
</script>
