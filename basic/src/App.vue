<template>

  <div>
    <HomeHeader /><hr>
    <BaseProject />
    <LifeCycle />
    <PersonApp />
  </div>

</template>

<script>

import BaseProject from './components/BaseProject.vue'
import HomeHeader from './components/HomeHeader.vue'
import LifeCycle from './components/LifeCycle.vue'
import PersonApp from './components/PersonApp.vue'

export default {
  name: 'App',

  components: {
    BaseProject,
    HomeHeader,
    LifeCycle,
    PersonApp,
}
}
</script>


<style>
  body {
    background-color: #333;
    color: #FFF;
  }

  a {
    color: blue;
    text-decoration: none;
    
  }

  .portfolio {
    color: aquamarine
  }
</style>
