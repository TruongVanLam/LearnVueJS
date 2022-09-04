<script>
import Todo from './components/todo.vue'
import Counter from './components/counter.vue'
import EventHandling from './components/event_handling.vue'
import Binding from './components/binding.vue'
export default {
  components: { Todo, Counter, EventHandling, Binding }
}
</script>

<template>
  <todo></todo>
  <counter></counter>
  <event-handling></event-handling>
  <br/>
  <binding></binding>
</template>
