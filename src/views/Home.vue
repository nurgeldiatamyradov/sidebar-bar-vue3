<template>
    <main class="home-page">
        <h1>home</h1>
        <p>sndbd</p>
    </main>
</template>

<script setup>
   async function getData() {
        const API = 'https://dog.ceo/api/breeds/image/random';
        let result = await fetch(API).then((response) => response.json())
        .then((response) => response)
       console.log(result)
    }

    getData();
 

</script>
