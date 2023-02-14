<template>
    <h1>home page:  {{ counterStore.counter}}</h1>
    <p> numero de cambios: {{ counterStore.numberOfChanges}}</p>
</template>

<script lang="ts" setup>
import { useCounterStore } from '../stores/counterStore';
const counterStore = useCounterStore();
</script>
