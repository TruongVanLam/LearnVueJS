<script>
    export default {
        data() {
            return {
                content: ""
            }
        },
        props: {
            post: {
                type: Object,
            }
        },
        methods: {
            handleChangeTitle() {
                return this.post.title = "Update complete!"
            }
        }
    }
</script>

<template>
    <h2> Thang con: {{post.title}}</h2>
    <button @click="handleChangeTitle()">Change title con</button>
</template>