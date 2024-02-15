<template>
    <div>
        <h2 class="thename">{{ Whale.name }}</h2>
        <img :src="Whale.img" alt="" class="image">
        <button @click="increment" class="thebutton">Add Whale</button>
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
.image {
    width: 15%;
    height: 15%;
    display: flex;
    flex-wrap: wrap;
    margin-top: 5px;

}

.thename{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    font-family: 'Manrope', sans-serif;
    margin-top: 10px;
}

.thebutton{
    display: flex;
    flex-wrap: wrap;
    font-family: 'Manrope', sans-serif;
}

</style>
