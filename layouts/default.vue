<script setup lang="ts">
import Navbar from '../components/Navbar.vue';
</script>

<template>
  <div class="min-h-screen bg-base-200/60">
    <Navbar />
    <div class="p-6">
      <slot />
    </div>
  </div>
</template>
