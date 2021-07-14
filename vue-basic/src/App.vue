<template>
  <div>
    <h4>ini parent components</h4>
    <child-component text="test123" />
    <child-component :text="message" />
  </div>
</template>

<script>
import ChildComponent from './components/ChildComponent.vue';
export default {
  components: { ChildComponent },
  data() {
    return {
      message: 'halo bro',
    };
  },
};
</script>
