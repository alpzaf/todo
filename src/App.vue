<template>
  <Container/>
  <Input @addTodoEnter="addTodoEnter" @addTodo="addTodo" />
  <Todos :todos="todos" v-for="todos in todoList" :key="todos.id"/>
</template>

<script>
import Container from './components/Container.vue'
import Todos from './components/Todos.vue'
import Input from './components/Input.vue'

export default {
  components : {
    Container,
    Todos,
    Input
  },
  data() {
    return {
      todoList: [
        {
          id: 1,
          content: 'yapılacaklar 1'
        },
        {
          id: 2,
          content: 'yapılacaklar 2'
        },
        {
          id: 3,
          content: 'yapılacaklar 3'
        },
        {
          id: 4,
          content: 'yapılacaklar 4'
        },
        {
          id: 5,
          content: 'yapılacaklar 5'
        },
        {
          id: 6,
          content: 'yapılacaklar 6'
        }
      ]
    }
  },
  methods : {
    addTodoEnter(todo) {
      console.log(todo)
    },
    addTodo(todo) {
      console.log(todo)
    }
  }
}
</script>