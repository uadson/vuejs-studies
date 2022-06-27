<template>
    <div>
        <form action="" @submit="sendData($event)">
            <div>
                <div>
                    <label for="">Name</label>
                </div>
                <div>
                    <input type="text" v-model="name">
                </div>
            </div>
            <div>
                <div>
                    <label for="">Email</label>
                </div>
                <div>
                    <input type="email" v-model="email">
                </div>
            </div>
            <div>
                <ButtonSubmit />
            </div>
        </form>
    </div><hr>
</template>

<script>
    //import InputText from './form/InputText.vue'
    import ButtonSubmit from './form/ButtonSubmit.vue'

    export default {
        name: 'UserForm',
        components: {
        //    InputText,
            ButtonSubmit,
        },
        data(){
            return {
                name: '',
                email: '',
            }
        },
        methods: {
            sendData(e){
                e.preventDefault();
                const name = this.name;
                const email = this.email;
                console.log('Send Form');
                console.log(`Name is ${name}`);
                console.log(`Email is ${email}`);
            }
        }
    }
</script>