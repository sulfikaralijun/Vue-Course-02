<script setup>
  import { useCounterStore }from '../stores/counter.js'
  const count = useCounterStore()
</script>

<template>
  <div>
    <p>Double: {{ count.doubleCount }}</p>
  
  </div>
</template>