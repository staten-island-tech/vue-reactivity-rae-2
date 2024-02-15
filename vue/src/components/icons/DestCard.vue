<template>
    <div>
        <h2>{{ Whale.name }}</h2>
        <img :src="Whale.img" alt="" class="image">
        <button @click="increment">Add Whale</button>
        <h3>{{ clicked }}</h3>
    </div>
</template>

<script setup>
import {ref} from "vue";
const props = defineProps({
    Whale: Object,
});

//clicker logic
const clicked = ref(0);
function increment(){
    clicked.value++;
}
</script>

<style scoped>
img {
    width: 300px;
    height: 300px;

}

</style>
