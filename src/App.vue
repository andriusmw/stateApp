<script setup>
import {ref} from "vue"

const red = ref(0)
const blue = ref(0)
const green = ref(0)

</script>


<template>
    <main :style="{backgroundColor: `rgb(${red},${green},${blue})`}">
      <div>
        <!-- v-model was two way data binding -->
        <input type="number" v-model="red"    placeholder="red">
        <input type="number" v-model="blue"   placeholder="blue">
        <input type="number" v-model="green"  placeholder="green">
      </div>
        
    </main>
</template>



<style scoped>

  main {
   
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

div {
  display: flex;
  flex-direction: column ;
}
</style>
