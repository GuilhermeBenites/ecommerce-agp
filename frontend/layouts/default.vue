<template>
  <div class="min-h-screen bg-neutral-100">
    <Header />
    <slot />
  </div>
</template>

<script lang="ts" setup>
import Header from '@/components/layout/Header.vue'
</script>

<style></style>