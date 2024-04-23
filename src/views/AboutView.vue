<script setup>
  import { useCounterStore }from '../stores/counter.js'
  import Result from "../components/Result.vue"
  const count = useCounterStore()
</script>


<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>{{ count.count }}</p>
    <button @click="count.increment()">Single</button>
    <Result/>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
