<template>
  <h2 v-if="status">Ini contoh dari if else</h2>
  <button @click="setStatus">toggle</button>
  <h3 v-if="status">True</h3>
  <h3 v-else-if="status2">False</h3>
  <h3 v-else>WASD</h3>
</template>

<script>
export default {
  data() {
    return {
      status: false,
      status2: true,
    };
  },
  methods: {
    setStatus() {
      this.status = !this.status;
    },
  },
};
</script>
