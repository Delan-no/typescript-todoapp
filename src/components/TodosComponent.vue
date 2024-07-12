<template>
  <div>
    <!-- Header -->
    <Header />

    <!-- TodoMain -->
    <TodoMain />

    <!-- TodoFooter -->
    <TodoFooter />
  </div>
</template>

<script setup lang="ts">
import Header from '@/components/TodoHeader.vue'
import TodoMain from '@/components/TodoMain.vue'
import TodoFooter from '@/components/TodoFooter.vue'
</script>

<style scoped></style>
