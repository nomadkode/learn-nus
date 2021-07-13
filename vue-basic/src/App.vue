<template>
  <div>{{ count }}</div>

  <button @click="count++">Add 1</button>
  <button @click="addCount">Add Count</button>
</template>

<script>
export default {
  data() {
    return {
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
