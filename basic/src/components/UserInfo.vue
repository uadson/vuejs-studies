<template>
    <div>
        <div>
            <p>{{ location }}</p>
            <p v-if="is_working"> I'm working</p>
            <p v-else>I'm looking for news oportunities</p>
            <p>I used the technologies for backend:</p>
        </div>
        <div>
            <!-- V-FOR -->
            <ul style="list-style: none;">
                <li v-for="(tech, index) in backend" v-bind:key="index">
                    {{ tech }}
                </li>
            </ul>
        </div>
        <div>
            <p>And I used the technolies for frontend:</p>
        </div>
        <div>
            <ul style="list-style: none;">
                <li v-for="tech in frontend" :key="tech.id">
                    {{ tech.framework }}
                </li>
            </ul>
            <!-- -->
        </div>
        <div>
            <MultEvents />
        </div>
        <div>
            <MyPictures />
            <p class="portfolio">To access my portfolio <a v-bind:href="portfolio" target="_blank">click here</a></p>
        </div>
        <div>
            <button @click="showEmail">{{ btnText }}</button>
        </div>
        <div>
            <h4 v-show="show_email">Send an email to: {{ email }}</h4>
        </div>
    </div>
</template>

<script>
import MyPictures from './MyPictures.vue'
import MultEvents from './MultEvents.vue'

export default {
    name: 'UserInfo',
    
    components: {
        MultEvents,
        MyPictures,
    },
    
    props: {
        location: String,
        is_working: Boolean
    },

    data(){
        return{
            show_email: false,
            email: 'uadson@uadson.com',
            portfolio: 'https://github.com/uadson',
            btnText: 'Show Email',
            // list or array
            backend: ['Python', 'Django', 'Django Rest Framework'],
            // dict or objects
            frontend: [
                {
                    id:1,framework: 'Vue',
                }
            ]
        }
    },
    methods: {
        showEmail() {
            this.show_email = !this.show_email
            if(!this.show_email){
                this.btnText = 'Show Email'
            } else {
                this.btnText = 'To Hide Email'
            }
        }
    }
}
</script>