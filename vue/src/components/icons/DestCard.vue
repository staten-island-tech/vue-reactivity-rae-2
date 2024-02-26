<template>
    <div class="poop">
        <h2 id="thename">{{ Whale.name }}</h2>
        <img :src="Whale.img" alt="" id="image">
        <button @click="increment" id="thebutton">Add Whale</button>
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

.poop{
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    font-family: 'Manrope', sans-serif;
    margin-top: 10px;
}

#thename{
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    font-family: 'Manrope', sans-serif;
    margin-top: 10px;
}

#image{
    width: 35%;
    height: 35%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
}
#thebutton{
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    font-family: 'Manrope', sans-serif;
}

</style>
