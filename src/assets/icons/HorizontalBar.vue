<template>
  <svg
    :width="width"
    height="2"
    :viewBox="`0 0 ${width} 2`"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path :d="`M0 1L${width} 0.999984`" stroke="white" stroke-width="2" />
  </svg>
</template>

<script setup lang="ts">
defineProps<{
  width: number
}>()
</script>
