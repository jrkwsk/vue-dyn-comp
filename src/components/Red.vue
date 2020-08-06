<template>
    <div>
        <h1 slot="redSlot">red slot title</h1>
        <p slot="redSlot">red slot desc</p>
    </div>
</template>

<script></script>

<style scoped>
    div {
        border: 1px solid red;
        background-color: lightcoral;
        padding: 30px;
        margin: 20px auto;
        text-align: center;
        color: darkred;
    }
</style>