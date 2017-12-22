<template>
  <div class="header">
    <img src="../assets/me.png"/>
    <div class="brand"> {{ statement }} </div>
  </div>
</template>


<script>
export default {
  name: 'Header',
  data() {
    return {
      statement:
        'I am a full-stack developer who enjoys finding creative solutions to complex problems. Through passion, adaptability, and relentlessness, I am excited to bring visions to life and assert that nothing is impossible.'
    }
  }
}
</script>

<style scoped>
.header {
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  margin: 0 auto;
}

.brand {
  display: flex;
  align-items: center;
  width: 500px;
}

img {
  width: 250px;
  height: 250px;
  padding-right: 30px;
}


</style>
