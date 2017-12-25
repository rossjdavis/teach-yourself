<template>
  <div class="wrapper">
    <img src="../assets/me.png"/>
    <div class="brand">
      <div class='statement'> {{ statement }} </div>
      <nav>
        <a href="/#/">Home</a>
        <a href="/#/resume">Resume</a>
      </nav>
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

div, nav {
  display: flex;
  flex-direction: row;
}

.brand {
  justify-content: center;
  align-items: center;
  width: 500px;
  flex-direction: column;
}

.statement {
  border-bottom: 1px solid black;
  border-top: 1px solid black;
  padding: 20px 0;
  text-align: center;
  margin-top: 40px;
}

nav {
  padding-top: 20px;
}

a {
  padding: 0 10px;
  text-decoration: none;
  color: black;

}

a:hover {
  font-weight: 700;
}


img {
  width: 250px;
  height: 250px;
  border: 1px solid white;
  border-radius: 125px;
  margin-right: 30px;
}

.wrapper {
  justify-content: center;
}


</style>
