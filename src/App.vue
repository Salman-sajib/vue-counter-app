<script setup>
  import {ref} from "vue";
  const count = ref(0);
</script>

<template>
  <main>
    <div>
      <h4>The current count is....</h4>
      <h1>{{ count }}</h1>
      <button @click="count--">increase</button>
      <button @click="count++">reduce</button>
    </div>
  </main>
</template>

<style scoped>
 main {
  background-color: aliceblue;
  color: black;
  height: 100vh;
  width: 100vw;
  display: grid;
  place-items: center;
 }

 div {
  background-color: white;
  color: black;
  box-shadow: 2px 5px 20px rgba(33, 33, 33, 0.1);
  padding: 6rem 4rem;
  border-radius: 2rem;
  text-align: center;
 }

 h1 {
  font-size: 4rem;
  font-weight: 500;
  margin-block: 3rem;
 }

 h4 {
  font-size: 1.6rem;
  font-weight: 500;
 }
 
 button {
  border: none;
  border-radius: 20rem;
  outline: none;
  font-size: 1rem;
  text-transform: uppercase;
  background-image: linear-gradient(210deg, rgba(4,149,255,1.00) 0%,rgba(86,153,247,1.00) 100%);
  background-position: center center;
  color: black;
  margin-inline: .5rem;
  padding: 1rem 1.5rem;
  cursor: pointer;
  transition: all 300ms ease;
 }

 button:hover {
  background-image: linear-gradient(60deg, rgba(61,114,234,1.00) 0%,rgba(221,142,255,1.00) 100%);
  background-position: center center;
 }
</style>