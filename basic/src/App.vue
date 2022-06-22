<template>

  <div>
    <BaseProject/>
    <LifeCycle/>
  </div>

</template>

<script>

import BaseProject from './components/BaseProject.vue'
import LifeCycle from './components/LifeCycle.vue'

export default {
  name: 'App',

  components: {
    BaseProject,
    LifeCycle,
}
}
</script>
