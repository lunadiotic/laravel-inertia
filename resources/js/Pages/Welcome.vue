<template>
    <h1>Hello, Vue</h1>
    <h4>Welcome to, {{ appName }}</h4>
    <p>This is from inertia Page. visit another page</p>

    <Link :href="route('page')">Page</Link>
</template>

<script>
import { computed } from "vue";
import { usePage, Link } from "@inertiajs/inertia-vue3";

export default {
    components: {
        Link,
    },

    setup() {
        const appName = computed(() => usePage().props.value.appName);

        return { appName };
    },
};
</script>

<style></style>
