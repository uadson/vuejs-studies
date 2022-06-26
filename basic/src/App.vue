<template>

  <div>
    <BaseProject/>
    <LifeCycle/>
    <PersonApp/>
  </div>

</template>

<script>

import BaseProject from './components/BaseProject.vue'
import LifeCycle from './components/LifeCycle.vue'
import PersonApp from './components/PersonApp.vue'

export default {
  name: 'App',

  components: {
    BaseProject,
    LifeCycle,
    PersonApp,
}
}
</script>
