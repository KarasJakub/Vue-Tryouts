<template>
    <header>
        <h1>{{ title }}</h1>
        <AddButton text="Add Task" color="green"/>
    </header>
</template>

<script>
import AddButton from "./Button.vue"

    export default {
        name: "MainHeader",
        props: {
            title: String
        },
        components: {
            AddButton
        }
    }
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>