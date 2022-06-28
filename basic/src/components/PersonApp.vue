<template>
    <div>
        <h3>This is a description about person: {{ person }}</h3>
        <UserInfo :location="location" :is_working='false' /><hr>
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
                person: 'Uadson',
                location: "I'm from Goiânia, Goiás, Brazil."
            }
        }
    }
</script>