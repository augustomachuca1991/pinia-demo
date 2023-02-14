<template>
    <h1>counter page: {{counterStore.counter}}</h1>
    <button @click="increment(1)">+1</button>
    <button @click="increment(2)">+2</button>
    <button @click="increment(5)">+5</button>
</template>

<script lang="ts" setup>
import { useCounterStore } from '../stores/counterStore';


const counterStore = useCounterStore();

const increment = (value : number) => {
    counterStore.incrementBy(value);
}

</script>