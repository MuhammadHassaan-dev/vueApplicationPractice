<template>
    
     <h2>Name is {{name}}</h2>
     {{shoePrevName != false ? "previous name is"+prevName : null}}
     <!-- <input
         :value="setName"
         @change="event => setName = event.target.value"> -->
         <input v-model="setName" />
     <button @click="changeName(setName)">change Name</button>
     <button @click="SetPreviousName">Set Previous Name</button>
   
</template>
<script setup lang="ts">
import {ref,watch} from 'vue';
const setName=ref("");
const name=ref("ALi Hamza");
const prevName=ref(" ");
const shoePrevName=ref(false);
// watch(name,()=>{
  
// })(
const SetPreviousName=()=>{
    shoePrevName.value=!shoePrevName.value
}
const changeName=(n)=>{
    console.log(n);
    prevName.value=name.value
    name.value=n;
}
</script>