<template>
    <div>
        <p v-if="is_working"> I'm working</p>
        <p v-else>I'm looking for news oportunities</p>
        <p>I used the tecnologies:</p>
        <ul>
            <li>Python</li>
            <li>Javascript</li>
        </ul>
        <div>
            <MyPictures />
            <p>To access my portfolio <a v-bind:href="portfolio" target="_blank">click here</a></p>
        </div>
    </div>
</template>

<script>
import MyPictures from './MyPictures.vue'

export default {
    name: 'UserInfo',
    components: {
        MyPictures,
    },
    data(){
        return{
            is_working: true,
            portfolio: 'https://github.com/uadson'
        }
    }
}
</script>