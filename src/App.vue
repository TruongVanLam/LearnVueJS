<script>
import Todo from './components/todo.vue'
import Counter from './components/counter.vue'
import EventHandling from './components/event_handling.vue'
import Binding from './components/binding.vue'
import Props from './components/props.vue'
export default {
  components: { Todo, Counter, EventHandling, Binding, Props },
  data() {
    return {
        post: {
            id: 1,
            title: 'My life is best than'
        },
        favorited: true,
    }
  },
}
</script>

<template>
  <todo></todo>
  <counter></counter>
  <event-handling></event-handling>
  <br/>
  <binding></binding>
  <props v-bind:post="post"></props>
  <button @click="post.title = 'update'">Change title cha</button>
  <p> Thang cha: {{post.title}}</p>
</template>
