<template>
  <div>
    <load-header/>
    <show-skills/>
    <show-xp/>
    <show-education/>
  </div>
</template>


<script>
import Header from './Header'
import Skills from './Skills'
import Experience from './Experience'
import Education from './Education'
export default {
  name: 'Resume',
  components: {
    'load-header': Header,
    'show-skills': Skills,
    'show-xp': Experience,
    'show-education': Education
  }
}
</script>

<style scoped>
</style>
