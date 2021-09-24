<template>
    <h1>Hello, Vue</h1>
    <p>This is from inertia Page. visit another page</p>

    <Link :href="route('page')">Page</Link>
</template>

<script>
import { Link } from "@inertiajs/inertia-vue3";

export default {
    components: {
        Link,
    },
};
</script>

<style></style>
