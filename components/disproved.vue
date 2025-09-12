<template>
    <li class="good" v-click.hide="'+1'"><slot /></li>
    <li class="bad" v-click="'+0'"><slot name="disproof" /></li>
</template>

<style>
    .good {
        position: absolute;
        color: red;
    }
    .good::marker {
        content: "× ";
    }
</style>