<template>
  <div>
    <ul>
      <li v-for="(todo, index) in todos" :key="todo.id">
        {{ index }} - {{ todo.activity }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        { id: 1, activity: 'wake up' },
        { id: 2, activity: 'code' },
        { id: 3, activity: 'sleep' },
      ],
    };
  },
};
</script>
