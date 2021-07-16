// V-Model = Two way data binding
<template>
  <div>
    <p>{{ message }}</p>
    <input v-model="message" />
    <!-- dibalik layar dr v-model -->
    <input :value="message" @input="message = $event.target.value" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'hi model',
    };
  },
};
</script>
