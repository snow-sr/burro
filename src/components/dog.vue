<!-- eslint-disable-next-line vue/multi-word-component-names -->
<template>
  <main :style="style">
    <h1>{{ name }}</h1>
    <p>{{ position }}</p>
  </main>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    position: {
      type: Array,
      required: true,
    },
  },

  computed: {
    style() {
      return `transform: translate(${this.position[0]}px, ${this.position[1]}px)`;
    },
  },
};
</script>

<style scoped>
* {
  color: RED;
}
</style>
