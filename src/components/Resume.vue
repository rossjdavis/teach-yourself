<template>
  <div>
    <load-header/>
    <show-skills/>
    <show-xp/>
  </div>
</template>


<script>
import Header from './Header'
import Skills from './Skills'
import Experience from './Experience'
export default {
  name: 'Resume',
  components: {
    'load-header': Header,
    'show-skills': Skills,
    'show-xp': Experience
  }
}
</script>

<style scoped>
</style>
