<template>
    <nav class="NavContain">
        <ul class="NavUl">
            <li>
                <NuxtLink to="/">Home</NuxtLink></li>
            <li>
                <NuxtLink to="/ToDo">Mis tareas</NuxtLink>    
            </li>
        </ul>        
    </nav>
</template>

<script setup>
</script>

<style lang="postcss">
.NavContain{
    display: flex;
    width:100%;
    height: 70px;
    border-bottom: solid 1px #afafaf;

    .NavUl{
        width: 100%;
        display: flex;
        justify-content: end;
        margin: 15px;

        li{
            width: 100px;
            border: solid 1px #afafaf;
            border-radius: 5px;
            margin-right: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    }
}
</style>