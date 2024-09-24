<script setup>
import { RouterLink, RouterView } from 'vue-router'
import nav_bar from './components/nav_bar.vue'
import side_bar from './components/side_bar.vue'
</script>

<template>
  <div class="header">
    <div class="navbar">
      <nav_bar />
    </div>
  </div>

  <!-- Main container to hold both sidebar and content -->
  <div class="main-container">
    <!-- Sidebar -->
    <div class="sidebar">
      <side_bar />
    </div>

    <!-- Body content -->
    <div class="body-content">
      <div class="nav-item">
        <div class="table">
          <RouterView />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Flexbox layout */
.main-container {
  display: flex; /* Aligns items horizontally */
}

.sidebar {
  width: 250px; /* Set a fixed width for the sidebar */
}
.body-content {
  flex-grow: 1; /* Body content will take the remaining width */
  padding: 50px; /* Add padding for space between content and sidebar */
}
</style>
