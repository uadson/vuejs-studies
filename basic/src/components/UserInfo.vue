<template>
    <div>
        <p v-if="is_working"> I'm working</p>
        <p v-else>I'm looking for news oportunities</p>
        <p>I used the tecnologies:</p>
        <ul>
            <li>Python</li>
            <li>Javascript</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'UserInfo',
    data(){
        return{
            is_working: true
        }
    }
}
</script>