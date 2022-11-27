<template>
    <button v-on:click="$emit('add', Math.random())">
        Add Math.random()
    </button>
</template>