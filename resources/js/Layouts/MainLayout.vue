<template>
    <Link href="/">Main Page</Link>&nbsp;
    <Link href="/hello">Show Page</Link>
    <!-- Persistent Layout to make a template of layouting -->
    <slot>Default</slot>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
</script>
