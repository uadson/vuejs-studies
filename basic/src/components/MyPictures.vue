<template>
    <img :src="avatar" :alt="description">
</template>

<script>
    export default {
        name: 'MyPictures',

        data() {
            return {
                avatar: '/img/avatar.png',
                description: 'Uadson Feitosa'
            }
        }
    }
</script>