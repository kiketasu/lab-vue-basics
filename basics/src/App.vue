<template>
  <Navbar />
    <button @click="show()">Calcular</button>
    <div v-if="isRender" class="calculator"><input type="number"> + <input type="number"> = {{result}}
</div>
  <Footer />
</template>
<script setup>
import  Navbar from "./components/Navbar.vue";
import  Footer from "./components/Footer.vue";
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
.calculator {
margin-left: 48%;
}
</style>