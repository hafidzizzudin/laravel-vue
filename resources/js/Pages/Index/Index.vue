<template>
    <div>Index</div>
    <Link href="/hello">Show Page</Link>
    <!-- interpolation syntax or master syntax {{  }} -->
    <div>The message is {{ message }}</div>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
// prop declaration https://vuejs.org/guide/components/props.html
defineProps({
    message: {
        type: String,
        required: true,
    },
});
</script>
