<template>
    <main>
        <h1>Mi lista ToDo</h1>

        <section class="ToDoContainer">
            <ToDoCard
            v-for="(tarea, index) in ToDoData"
            :key="index"
            :tarea="tarea"/>
        </section>
        <InputToDo/>
    </main>
</template>

<script setup>

import{ref} from 'vue'
const ToDoData=ref([
    {
        id:1,
        name: "Tirar basura",
        time:"12am",
        img:"https://picsum.photos/200/500" 
    },
    {
        id:2,
        name: "Hacer colada",
        time:"3pm",
        img:"https://picsum.photos/200/400"
    },
    {
        id:3,
        name: "Hacer deberes",
        time:"5pm",
        img:"https://picsum.photos/100/300"
    },
    {
        id:4,
        name: "Cita médica",
        time:"6:30pm",
        img:"https://picsum.photos/200/300" 
    },
    {
        id:5,
        name: "Cena familiar",
        time:"8:30pm",
        img:"https://picsum.photos/200/200"
    },
    {
        id:6,
        name: "Netflix & chill",
        time:"9:30pm",
        img:"https://picsum.photos/300/300"
    },
]);

</script>

<style lang="postcss">
.ToDoContainer{
    display: grid;
    grid-template-columns: 1fr 1fr;

}

</style>