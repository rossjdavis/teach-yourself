<template>
  <div>
    <load-header/>
    <show-projects/>
  </div>
</template>


<script>
import Header from './Header'
import Projects from './Projects'
export default {
  name: 'Home',
  components: {
    'load-header': Header,
    'show-projects': Projects
  }
}
</script>

<style scoped>
</style>
