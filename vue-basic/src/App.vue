<template>
  <div>
    <declarative />
    <vmodel />
    <vif />
    <vfor />
    <child-component text="tesprops" />
    <child-component :text="pesan" />
    <child-component v-for="todo in todos" v-bind:key="todo" :text="todo" />
    <lifecycle />
  </div>
</template>

<script>
import Declarative from './components/Declarative.vue';
import Vmodel from './components/Vmodel.vue';
import Vif from './components/Vif.vue';
import Vfor from './components/Vfor.vue';
import ChildComponent from './components/ChildComponent.vue';
import Lifecycle from './components/Lifecycle.vue';

export default {
  components: { Declarative, Vmodel, Vif, Vfor, ChildComponent, Lifecycle },
  data() {
    return {
      pesan: 'halo dunia',
      todos: ['pertama', 'kedua', 'ketiga'],
    };
  },
};
</script>

<style>
body {
  background-color: #0c0b36;
  color: #f1f1f1;
}

h1,
h2,
h3,
p {
  display: flex;
  justify-content: center;
  align-items: center;
}

ul {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

button {
  margin: 0.5rem auto;
  padding: 1rem;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #010101;
  color: #f1f1f1;
  outline: none;
  border: none;
  border-radius: 10px;
}

button:hover {
  transform: scale(1.1);
}

input {
  margin: 0.5rem auto;
  padding: 0.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
