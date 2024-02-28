<template>
  <div>
    <DestCard
    v-for="whale in whales" 
    :key="whales.name" 
    :Whale="whale"
    @click="addtoBowl(bowl)"><!--  i have no idea if this is it -->
  </DestCard>
  
  </div>
</template>

<script setup>
import DestCard from '@/components/icons/DestCard.vue';

const whales = [
        {
          name: "Baleen Whale",
          Big: true,
          img: "https://oceananimals.org/wp-content/uploads/2021/05/Humpback-Graphic-1-e1619925628948-1024x711.png",
        },
        {
          name: "Narwhal",
          Big: true,
          img: "https://images.squarespace-cdn.com/content/v1/62a5e640df138f7689bde14b/1655219797187-68BBLSTD0Y3WAAJ3UJ82/14B35550-E738-452A-984B-7F294510998E.jpeg?format=1000w",
        },
        {
          name: "Pilot Whale",
          Big: true,
          img: "https://www.northsailing.is/wp-content/uploads/2017/05/MC068grindhvalur.jpg",
        },
        {
          name: "Pygmy Sperm Whale",
          Big: false,
          img: "https://www.researchgate.net/publication/323780767/figure/fig10/AS:631577352605746@1527591183407/The-pygmy-sperm-whale-Kogia-breviceps-Illustration-from-Laura-Hedon.png",
        },
        {
          name: "Sei Whale",
          Big: true,
          img: "https://whaleopedia.org/animalfund/wp-content/uploads/2013/10/Sei-Whale1.png",
        },
        {
          name: "Whalen",
          Big: true,
          img: "https://3.files.edl.io/aeb1/20/12/02/154937-46cc468f-b7f4-4bb3-945e-3265bdb605d4.jpg",
        },
      ];

</script>

<style scoped>

</style>
