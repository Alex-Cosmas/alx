<template>
  <button
    @click="onClick()"
    class="btn text-white text-white rounded-md shadow-sm px-8 py-2"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String
  },
  methods: {
    onClick() {
      // console.log('clicked');
      this.$emit('toggle-add');
    }
  }
};
</script>
