<template>
  <div class="flex flex-col justify-center items-center min-h-screen">
    <Header />
    <Main>
      <ListTodos color="green" title="Pending Items" :todos="pendingTodos" />
      <ListTodos color="red" title="Completed Items" :todos="completedTodos" />
    </Main>
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import ListTodos from './components/ListTodos.vue'
import { pendingTodos, completedTodos } from './helpers/useTodos'
</script>
