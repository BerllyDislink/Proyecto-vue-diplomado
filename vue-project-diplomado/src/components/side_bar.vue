<script setup>
import { ChevronRightIcon } from '@heroicons/vue/24/solid'
</script>
<template>
  <nav class="sidebar sidebar-offcanvas" id="sidebar">
    <ul class="nav">
      <li class="nav-item">
        <RouterLink class="nav-link" to="index">
          <i class="icon-grid menu-icon"></i>
          Inicio</RouterLink
        >
      </li>
      <li class="nav-item">
        <RouterLink class="nav-link" to="/table">
          <i class="icon-layout menu-icon"></i>
          <span class="menu-title">Listado</span>
          <ChevronRightIcon class="ChevronRight"></ChevronRightIcon>
        </RouterLink>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          data-bs-toggle="collapse"
          href="#icons"
          aria-expanded="false"
          aria-controls="icons"
        >
          <i class="icon-contract menu-icon"></i>
          <span class="menu-title">Icon</span>
          <ChevronRightIcon class="ChevronRight"></ChevronRightIcon>
        </a>
        <div class="collapse" id="icons">
          <ul class="nav flex-column sub-menu">
            <li class="nav-item">
              <a class="nav-link" href="../pages/icons/mdi.html">Mdi icons</a>
            </li>
          </ul>
        </div>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="../index.html">
          <i class="icon-head menu-icon"></i>
          <span class="menu-title">User Pages</span>
          <ChevronRightIcon class="ChevronRight"></ChevronRightIcon>
        </a>
        <div class="collapse" id="auth">
          <ul class="nav flex-column sub-menu">
            <li class="nav-item">
              <a class="nav-link" href="../pages/samples/login.html"> Login </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="../pages/samples/register.html"> Register </a>
            </li>
          </ul>
        </div>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          data-bs-toggle="collapse"
          href="#error"
          aria-expanded="false"
          aria-controls="error"
        >
          <i class="icon-ban menu-icon"></i>
          <span class="menu-title">Error pages</span>
          <ChevronRightIcon class="ChevronRight"></ChevronRightIcon>
        </a>
        <div class="collapse" id="error">
          <ul class="nav flex-column sub-menu">
            <li class="nav-item">
              <a class="nav-link" href="../pages/samples/error-404.html"> 404 </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="../pages/samples/error-500.html"> 500 </a>
            </li>
          </ul>
        </div>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="../../../docs/documentation.html">
          <i class="icon-paper menu-icon"></i>
          <span class="menu-title">Documentation</span>
          <ChevronRightIcon class="ChevronRight"></ChevronRightIcon>
        </a>
      </li>
    </ul>
  </nav>
</template>
