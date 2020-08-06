<template>
    <div>
        <h1 slot="greenSlot">green slot title</h1>
        <p slot="greenSlot">green slot desc</p>
    </div>
</template>

<script>

</script>

<style scoped>
    div {
        border: 1px solid green;
        background-color: lightgreen;
        padding: 30px;
        margin: 20px auto;
        text-align: center;
        color: darkgreen;
    }
</style>