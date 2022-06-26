<template>
    <div>
        <h3>This is a description about person: {{ person }}</h3>
        <UserInfo /><hr>
        <UserForm />
    </div>
</template>

<script>
    import UserForm from './UserForm.vue'
    import UserInfo from './UserInfo.vue'
    
    export default {
        name: 'PersonApp',
        components: {
            UserInfo,
            UserForm,
        },
        data(){
            return{
                person: 'Uadson'
            }
        }
    }
</script>