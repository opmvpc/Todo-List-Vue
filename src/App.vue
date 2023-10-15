<script setup>
import { ref } from 'vue';

const taches = ref([]);
const tache = ref('');

const ajouter = () => {
  taches.push(tache);
  tache.value = '';
};
</script>

<template>
  <nav class="navbar bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Todo List</a>
    </div>
  </nav>

  <div class="container">
    <div class="mb-3">
      <label for="tache" class="form-label">Tâche</label>
      <input
        type="text"
        class="form-control"
        id="tache"
        placeholder="Un truc à faire"
      />
    </div>
  </div>
</template>

<style scoped></style>
