<template>
    <div>
        <h4 v-show="email">Send an email to: {{email}}</h4>
        <form action="">
            <div>
                <label for="">Name</label>
                <InputText />
            </div>
            <div>
                <label for="">Email</label>
                <InputText />
            </div>
            <div>
                <ButtonSubmit />
            </div>
        </form>
    </div>
</template>

<script>
    import InputText from './form/InputText.vue'
    import ButtonSubmit from './form/ButtonSubmit.vue'

    export default {
        name: 'UserForm',
        components: {
            InputText,
            ButtonSubmit,
        },
        data() {
            return {
                email: 'uadson@uadson.com',
            }
        }
    }
</script>