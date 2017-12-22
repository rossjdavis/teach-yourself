<template>
  <div class="skills">
    <h3>Skills</h3>
    <div class="items">
      <p v-for="skill in skills">
        {{ skill.skill }}
      </p>
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
        { skill: 'ActiveRecord' }
      ]
    }
  }
}
</script>

<style scoped>
.skills {
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  margin: 0 auto;
}

.items {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  width: 500px;
}

h3 {
  display: flex;
  align-items: center;
  width: 250px;
  justify-content: center;
  padding-right: 30px;
}

p {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  padding: 0 9px;

}

</style>
