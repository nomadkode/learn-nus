<template>
  <div>
    <ol>
      <li v-for="(todo, index) in todos" :key="todo.id">
        {{ index }} - {{ todo.action }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        { id: 1, action: 'wake up' },
        { id: 2, action: 'learn' },
        { id: 3, action: 'sleep' },
      ],
    };
  },
};
</script>
