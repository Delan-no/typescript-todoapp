<template>
  <main class="main">
    <ul class="todo-list">
      <li :class="{ completed: todo.completed }" v-for="todo in taches" :key="todo.id">
        <div class="view">
          <input type="checkbox" class="toggle" />
          <label for="">{{ todo.title }}</label>
          <button class="destroy"></button>
        </div>
      </li>
    </ul>
  </main>
</template>

<script setup lang="ts">
import 'todomvc-app-css/index.css'
interface Todo {
  id: number
  title: string
  completed: boolean
}
// const props = defineProps(['taches'])
const props = defineProps<{
  taches: Todo[]
}>()
</script>

<style scoped></style>
