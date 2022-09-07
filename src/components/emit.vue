<script>
    export default {
        props: {
            post: {
                type: Object
            }
        },
        data() {
            return {
                mau: this.post.mau
            }
        }
    }
</script>

<template>
    <h2>$Emit</h2>
    <h4>{{post.title}}</h4>
    <button @click="this.$emit('change-color')">Change color</button>
</template>