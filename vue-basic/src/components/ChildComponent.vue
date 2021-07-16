<template>
  <div>
    <h3>Ini adalah child component</h3>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: '',
    },
  },
};
</script>
