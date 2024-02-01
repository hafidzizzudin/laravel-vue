<template>
    <Link href="/">Main Page</Link>&nbsp;
    <Link href="/hello">Show Page</Link>
    <div>The page with time {{ timer }}</div>
    <!-- Layout to make a template of layouting -->
    <slot>Default</slot>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
import { ref } from "vue";

// reactive variable ref
const timer = ref(0);

setInterval(() => {
    timer.value++;
    if (timer.value % 10 === 0) {
        timer.value = 0;
    }
}, 1000);
</script>
