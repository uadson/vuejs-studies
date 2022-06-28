<template>

  <div>
    <HomeHeader :is_logged='true' /><hr>
    <ReusableVue />
    <BaseProject />
    <ReusableVue />
    <LifeCycle />
    <ReusableVue />
    <PersonApp />
    <ReusableVue />
  </div>

</template>

<script>

import BaseProject from './components/BaseProject.vue'
import HomeHeader from './components/HomeHeader.vue'
import LifeCycle from './components/LifeCycle.vue'
import PersonApp from './components/PersonApp.vue'
import ReusableVue from './components/ReusableVue.vue'

export default {
  name: 'App',

  components: {
    BaseProject,
    HomeHeader,
    LifeCycle,
    PersonApp,
    ReusableVue,
},

}
</script>


<style>
  body {
    background-color: #333;
    color: #FFF;
    font-family: sans-serif;
  }

  a {
    color: blue;
    text-decoration: none;
    
  }

  .portfolio {
    color: aquamarine
  }
</style>
