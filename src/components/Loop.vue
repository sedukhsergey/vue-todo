<template>
  <div>
    <ol>
      <li v-for="todo in todos" v-bind:key="todo.id">
        <Todo :text="todo.text" />
      </li>
    </ol>
  </div>
</template>

<script>

import Todo from "@/components/Todo";

export default {
  components: {
    Todo,
  },
  data() {
    return {
      todos: [
        { id: 1, text: 'Learn JavaScript' },
        { id: 2, text: 'Learn Vue' },
        { id: 3, text: 'Build something awesome' }
      ]
    }
  }
}
</script>
