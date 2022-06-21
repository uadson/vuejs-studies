<template>
    <div>
        <h1>This is Vue JS</h1><hr>
        <h3>Introdution</h3>
        <p>Hello, my name is {{ name }} and I'm studing {{ framework[0] }}.<br>
           I'm {{ area }} {{ occupation }} and I programing with {{ language }}<br>
           and framework {{ framework[1]}}.
        </p>
    </div>
    
</template>

<script>
export default {
    name: 'BaseProject',
    data() {
        return {
            name: "Uadson",
            framework: ["Vue JS", "Django"],
            occupation: "Web Developer",
            area: "Backend",
            language: "Python",
        }
    }
}
</script>