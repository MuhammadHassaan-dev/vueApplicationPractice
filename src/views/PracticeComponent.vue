<script setup lang="ts">
import PracticeView from "../components/PracticeView.vue";
let homeObj={
  no:84,
  address:"93B Johar town",
  area:"Address",
}
</script>
<template>
<div>
    <h1>This is Practice Compoennt</h1>
    <PracticeView library="NodeJS" :home="homeObj"> </PracticeView>
</div>
</template>

