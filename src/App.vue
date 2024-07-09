<script setup lang="ts">
import EventCard from './components/EventCard.vue'
</script>

<template>
  <div class="wrapper">
    <header>
      <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </header>
  <RouterView />
  </div>
  <div class="home">
    <EventCard />
  </div>
</template>