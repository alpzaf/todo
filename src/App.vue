<template>
  <Container/>
  <Todos :todo="todo" v-for="todo in todoList" :key="todo.id"/>
</template>

<script>
import Container from './components/Container.vue'
import Todos from './components/Todos.vue'

export default {
  components : {
    Container,
    Todos
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
        }
      ]
    }
  }
}
</script>