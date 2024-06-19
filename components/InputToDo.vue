<template>
    <div class="NewToDo">
        <input value="Escribe tarea">
        <button>Añadir</button>
    </div>
</template>

<script setup>

</script>

<style lang="postcss">
.NewToDo{
    width: 70%;
    display:flex;
    justify-content: center;
    align-items: center;
    height: 80px;
    margin: 30px;

    input{
        border: solid 1px #afafaf;
        width: 260px;
        height: 40px;
        border-radius: 20px;
        justify-content: center;
        text-align: center;
    }

    button{
        display: flex;
        background-color: #afafaf;
        height: 40px;
        align-items: center;
        justify-content: center;
        padding-right: 30px;
        padding-left: 30px;
        margin-left: 10px;
        border-radius: 20px;

    }
    
}
</style>