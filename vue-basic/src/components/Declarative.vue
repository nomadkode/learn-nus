// Declarative Rendering & Methods Components
<template>
  <div>
    <h1>{{ message }}</h1>
    <p :title="message">blablabla</p>
    <p>{{ count }}</p>
    <button @click="count++">count 1</button>
    <button @click="addCount">add count</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'hi world',
      count: 0,
    };
  },
  methods: {
    addCount() {
      this.count += 2;
    },
  },
};
</script>
