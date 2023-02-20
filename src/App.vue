<template>
  <h1>{{ message }}</h1>
  <h2 @click="increase">{{ count }}</h2>
  <HelloWorld />
</template>

<script>
import HelloWorld from '~/components/HelloWorld';
export default {
  components: {
    HelloWorld,
  },
  data() {
    return {
      message: 'Hello Vue!',
      count: 0,
    };
  },

  methods: {
    increase() {
      this.count += 1;
    },
  },
};
</script>

<style></style>
