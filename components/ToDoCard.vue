<template>
    <article class="ToDoElem" v-show="HideToDo">
        <img :src="tarea.img" alt="Imagen tarea">
        <div class="InfoToDo"><h3>{{ tarea.name }} at {{ tarea.time }}</h3></div>
        <button @click="HideToDo=!HideToDo"><h3>borrar</h3></button>
    </article>
</template>

<script setup>
import{ref} from 'vue'
const HideToDo=ref(true);

const props=defineProps({
    tarea: {
        type: Object,
        required: false
    }
});
const{tarea}=props;

</script>

<style lang="postcss">
.ToDoElem{
    width: 400px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border:solid 1px #afafaf;
    margin: 30px;
    border-radius: 10px;

    img{
        height: 80px;
        width: 80px;
        object-fit: cover;
        border-radius: 40px;
        margin: 10px;
    }

    .InfoToDo{
        margin: 10px;
    }

    button{
        height: 80px;
        width: 80px;
        margin: 10px;
        background-color: #afafaf;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 40px;
    }

    
}
</style>