<template>
  <div class="todo-input bg-gray-200 xl:container m-auto xl:rounded py-5 px-5 flex items-center mt-5" >
    <input v-model="todo" @keydown.enter="addTodoEnter" class="border-none bg-white xl:rounded w-10/12 px-5 py-5">
    <button @click="addTodo" class="w-44 block bg-gray-400 h-16 px-5 py-1 xl:rounded text-white ml-auto">+</button>
  </div>
</template>

<script>
  export default {
    data : function() {
      return {
        todo : ''
      }
    },
    methods : {
      addTodoEnter() {
        this.$emit('addTodoEnter', this.todo)
      },
      addTodo() {
        this.$emit('addTodo', this.todo)
      }
    }
  }
</script>