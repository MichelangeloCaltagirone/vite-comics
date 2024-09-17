<script>
    export default {
        data() {
            return {
            }
        },
        props: {
            picUrl: {
                type: String,
                required: true
            },
            price: {
                type: String,
                required: false
            },
            title: {
                type: String,
                required: true
            },
            bookType: {
                type: String,
                required: false
            }
        }

    }
</script>

<template>
    <h1>{{ title }}</h1>
</template>

<style scoped>
</style>