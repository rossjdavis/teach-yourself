<template>
  <div class="wrapper">
    <!-- <nav>
      <a href="/#/">Home</a>
      <a href="/#/resume">Resume</a>
    </nav> -->
    <h2>Ross Davis</h2>
    <div class="row">
      <img src="../assets/me.png"/>
      <div class="brand">
        <div class='statement'> {{ statement }} </div>
      </div>
    </div>
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

div {
  display: flex;
  flex-direction: column;
}

.row {
  flex-direction: row;
}

.brand {
  justify-content: center;
  align-items: center;
  width: 500px;
  flex-direction: column;
}

.statement {
  padding: 20px 0;
}

nav {
  padding-top: 20px;
}

a {
  padding: 0 10px;
  text-decoration: none;
  color: black;
}

img {
  width: 250px;
  height: 250px;
  border: 1px solid white;
  border-radius: 125px;
  margin-right: 15px;
}

h2 {
  text-align: left;
}

.wrapper {
  width: 750px;
  margin: 0 auto;
}


</style>
