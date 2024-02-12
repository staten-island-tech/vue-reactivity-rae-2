<template>
    <div>
        <h2>{{ Destination.name }}</h2>
        <img :src="Destination.img" alt="">
        <button @click="increment">Click Me</button>
        <h3>{{ clicked }}</h3>
    </div>
</template>

<script setup>
import {ref, reactive} from "vue";
const props = defineProps({
    Destination: Object,
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
