<template>
  <Container/>
  <Todos/>
</template>

<script>
import Container from './components/Container.vue'
import Todos from './components/Todos.vue'

export default {
  components : {
    Container,
    Todos
  }
}
</script>