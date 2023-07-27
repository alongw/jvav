<script setup lang="ts">
// import here ...
import NavComponents from '@/components/Nav.vue'
import UnderComponents from '@/components/Under.vue'

defineOptions({
  name: 'App'
})

// code here ...
</script>

<template>
  <nav-components />
  <router-view />
  <under-components />
</template>

