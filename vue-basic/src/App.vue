<template>
  <div>
    <h1 v-if="status">ini tampil</h1>
    <button @click="setStatus">toggle</button>
    <p v-if="status">true</p>
    <p v-else-if="status2">false</p>
    <p v-else>yes</p>
  </div>

  <!-- <div v-if="status">true</div>
  <div v-else-if="status2">false</div>
  <div v-else>yes</div> -->
</template>

<script>
export default {
  data() {
    return {
      message: 'hi world',
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
