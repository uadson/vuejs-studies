<template>
    <div>
        <h1>This is Vue JS</h1><hr>
        <h3>Introdution</h3>
        <p class="pg-main">Hello, my name is {{ name }} and I'm studing {{ framework[0] }}.<br>
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

<!-- Style in a component but it's not scoped (not recomendate)-->
<style>
  .pg-main {
    color: aquamarine
  }
</style>