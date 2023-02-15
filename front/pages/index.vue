//Create a fetch to f1 public api to extract data?
<script setup lang="ts">
import F1data from '~~/types/F1data'

const data: F1data = await fetch('https://ergast.com/api/f1/2021/1/driverStandings.json')
    .then(res => res.json())
    .catch(err => console.log(err))
    

</script>
<template>
    <div>
        <h1>Formula 1</h1>
        <p>{{data}}</p>
    </div>
</template>