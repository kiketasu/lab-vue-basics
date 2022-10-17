<template>
  <Navbar />
    <button @click="show()">Click para sorpresa</button>
    <div v-if="isRender" class="container">
      {{"Sorpresa"}}
</div>
<Data />
  <Footer />
</template>
<script setup>
import  Navbar from "./components/Navbar.vue";
import  Footer from "./components/Footer.vue";
import Data from "./components/Data.vue"
import {ref} from 'vue';
const isRender = ref(false);
const show = () => {
  isRender.value = !isRender.value;
}

</script>
<style scoped>

input {
  width: 50px;
}
button {
margin-left: 50%;
margin-bottom: 10px;
}
.container {
margin-left: 50%;
}

.color{
  background-color: blueviolet;
}

</style>