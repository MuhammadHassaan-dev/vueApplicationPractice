<template>
    <h1>Practice {{ library }}</h1>
    <h2>Home no : {{ home.no  }}</h2>
    <h2>Address is : {{ home.address  }}</h2>
</template>
<script lang="ts">
export default{
    props:{
        library:String,
        home:Object,
    },
};
</script>