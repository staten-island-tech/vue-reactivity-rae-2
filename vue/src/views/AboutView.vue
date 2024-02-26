<template>
  <div class="bowl">
    <h1>
      <img src="https://m.media-amazon.com/images/I/71rUwkdGglL.jpg" alt="" class="bowlimg">
    </h1>
  </div>
  
</template>

<script setup>
import { whales } from './HomeView.vue';
const whaleinbowls = new whales
</script>

<style>
  .bowlimg {
    max-width: 760px;
    max-height: 760px;
    display: flex;
    flex-wrap: wrap;
    margin-top: 100px;
  }
</style>
