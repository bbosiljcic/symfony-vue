<template>
    <span class="p-3">
        {{ title }}
    </span>
</template>

<script>
export default {
    name: 'BaseLegend',
    props: {
        title: {
            type: String,
        },
    },
};
</script>

<style scoped>

</style>
