<template>
  <q-page class="row items-center justify-evenly">
    <div>{{ $t('failed') }}</div>
    <div>{{ todos }}</div>
  </q-page>
</template>

<script setup lang="ts">
const res = await fetch('https://jsonplaceholder.typicode.com/todos/1');
const todos = await res.json();
</script>
