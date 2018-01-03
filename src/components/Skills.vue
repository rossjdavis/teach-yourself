<template>
  <div class="wrapper">
    <h3>Skills</h3>
    <div class="row">
      <div class="col"></div>
      <div class="items">
        <span v-for="skill in skills">
          {{ skill.skill }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
        { skill: 'JavaScript' },
        { skill: 'HTML' },
        { skill: 'CSS' },
        { skill: 'Ruby' },
        { skill: 'RAILS' },
        { skill: 'Sinatra' },
        { skill: 'Mongoose' },
        { skill: 'Express' },
        { skill: 'React' },
        { skill: 'Node' },
        { skill: 'MERN' },
        { skill: 'SQL' },
        { skill: 'noSQL' },
        { skill: 'MVC' },
        { skill: 'ActiveRecord' },
        { skill: 'Vue' }
      ]
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

.col {
  width: 250px;
}

.items {
  flex-flow: row wrap;
  width: 500px;
}


span {
  padding-left: 15px;
}

h3 {
  border-bottom: 1px solid black;
  text-align: left;
  margin-top: -5px;
}

.wrapper {
  width: 750px;
  margin: 0 auto;
}

</style>
