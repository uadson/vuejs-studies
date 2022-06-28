<template>
    <img :src="avatar" :alt="description">
    <ChangePicture @change-picture="methodChange"/>
</template>

<script>
    import ChangePicture from './ChangePicture.vue'

    export default {
        name: 'MyPictures',

        components: {
            ChangePicture,
        },

        methods:{
            methodChange() {
                this.avatar = '/img/avatar2.png'
            }
        },

        data() {
            return {
                avatar: '/img/avatar.png',
                description: 'Uadson Feitosa'
            }
        }
    }
</script>