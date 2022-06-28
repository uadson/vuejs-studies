<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#" v-show="is_logged">Profile</a></li>
    </ul>
</template>

<script>
export default {
    name: 'HomeHeader',

    props: {
        is_logged: Boolean,
    }
}
</script>

<!-- Scoped only for HomeHeader.vue-->
<style scoped>
    ul {
        list-style: none;
        display: flex;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
        font-weight: bold;
        font-family: sans-serif;
    }

    a:hover {
        color: turquoise;
    }
</style>