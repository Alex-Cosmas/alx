<template>
  <button
    @click="onClick()"
    class="btn text-white text-white rounded-md shadow-sm px-8 py-2 bg-main-blue"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String
  },
  methods: {
    onClick() {
      console.log("clicked");
    }
  }
};

// :style="{ background: color }"
</script>
