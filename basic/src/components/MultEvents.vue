<template>
    <div class="mult-e">
        <button class="btn" @click="first(txt1, $event), second(txt2, $event), third(txt3, $event), fourth(txt4, $event), fifth()">Show Technologies</button>
    </div>
    <div>
        <p>{{ technologies }}</p>
    </div>
</template>

<script>
export default {
    name: 'MultEvents',
    data(){
        return {
            technologies: '',
            txt1: 'Python',
            txt2: 'Django',
            txt3: 'Django Rest Framework',
            txt4: 'Vue JS',
        }
    },
    methods: {
        first(txt){
            this.technologies = txt;
        },
        second(txt){
            setTimeout(()=> this.technologies = txt, 1000)
        },
        third(txt){
            setTimeout(()=> this.technologies = txt, 2000)
        },
        fourth(txt){
            setTimeout(()=> this.technologies = txt, 3000)
        },
        fifth(){
            setTimeout(()=> this.technologies = "", 4000)
        }
    }
}
</script>

<style scoped>
    .mult-e {
        margin: 50px;
    }
    .btn {
         background-color: aquamarine;
         border-color: aquamarine;
         border: 0px;
         border-radius: 5px;
         width: 120px;
    }
</style>