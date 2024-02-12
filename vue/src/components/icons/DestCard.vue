<template>
    <div>
        <h2>{{ whale.name }}</h2>
        <img :src="whale.img" alt="">
        <button @click="increment">Add Whale</button>
        <h3>{{ clicked }}</h3>
    </div>
</template>

<script setup>
import {ref, reactive} from "vue";
const props = defineProps({
    whale: Object,
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
