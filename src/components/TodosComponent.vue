<template>
  <div>
    <!-- Header -->
    <Header />

    <!-- TodoMain -->
    <TodoMain :taches="todos" />

    <!-- TodoFooter -->
    <TodoFooter />
  </div>
</template>

<script setup lang="ts">
import Header from '@/components/TodoHeader.vue'
import TodoMain from '@/components/TodoMain.vue'
import TodoFooter from '@/components/TodoFooter.vue'

interface Todo {
  id: number
  title: string
  completed: boolean
}

const todos: Todo[] = [
  {
    id: 1,
    title: 'Tache 1',
    completed: true
  },
  {
    id: 2,
    title: 'Tache 2',
    completed: false
  },
  {
    id: 3,
    title: 'Tache 3',
    completed: false
  }
]
</script>

<style scoped></style>
