<script setup>
import { ref } from 'vue'

const awesome = ref(true)

function toggle() {
  awesome.value = !awesome.value
}
</script>

<template>
<button @click="toggle">Get Whales</button>
  <h1 v-if="awesome"><img src="https://m.media-amazon.com/images/I/71rUwkdGglL.jpg" alt="" class="bowlimg"></h1>
  <h1 v-else>You can't put whales in a goldfish bowl HAHAH </h1>
</template>

<style>
  .bowlimg {
    max-width: 760px;
    max-height: 760px;
    display: flex;
    flex-wrap: wrap;
    margin-top: 100px;
  }
</style>

