<template>
    <main>
        <h1>Inicio</h1>
        <div class="IndexSub"><h2>Tu web de tareas de confianza</h2></div>
        <div class="descriptIndex"><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p></div>
    </main>
</template>

<script setup>

</script>

<style lang="postcss">
Main{
    display: flex;
    flex-direction: column;
    align-items: center;

    h1{
        font-size: 8cap;
        font-weight: 600;
    }

    .IndexSub{
        display: flex;
        border-bottom: solid 1px #afafaf;
        width: 50%;
        justify-content: center;
        padding: 30px;

        h2{
            font-size: 3cap;
        }
    }

    .descriptIndex{
        margin-top: 40px;
        width: 70%;
        display: flex;
        align-items: center;
        text-align: center;
    }
}

</style>