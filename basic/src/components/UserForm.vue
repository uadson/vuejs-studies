<template>
    <form action="">
        <div>
            <InputText />
        </div>
        <div>
            <InputText />
        </div>
        <div>
            <ButtonSubmit />
        </div>
    </form>
</template>

<script>
    import InputText from './form/InputText.vue'
    import ButtonSubmit from './form/ButtonSubmit.vue'

    export default {
        name: 'UserForm',
        components: {
            InputText,
            ButtonSubmit,
        }
    }
</script>