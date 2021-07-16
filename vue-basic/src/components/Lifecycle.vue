<template>
  <div id="lifecycle">
    <h1>{{ message }}</h1>
    <button @click="message = 'text dirender ulang'">update</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'text awal',
    };
  },
  beforeCreate() {
    console.log('before create');
  },
  created() {
    console.log('created');
    console.log(this.message);
    console.log(document.getElementById('lifecycle'));
  },
  beforeMount() {
    console.log('before mount');
  },
  mounted() {
    console.log('mounted');
    console.log(this.message);
    console.log(document.getElementById('lifecycle'));
  },
  beforeUpdate() {
    console.log('before update');
    console.log(document.getElementById('lifecycle').textContent);
  },
  updated() {
    console.log('updated');
    console.log(document.getElementById('lifecycle').textContent);
  },
  beforeUnmount() {
    console.log('before unmount');
  },
  unmounted() {
    console.log('unmounted');
  },
};
</script>
