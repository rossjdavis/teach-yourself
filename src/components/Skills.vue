<template>
  <div class="wrapper">
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
        { skill: 'ActiveRecord' },
        { skill: 'Vue' }
      ]
    }
  }
}
</script>

<style scoped>

div, h3, p {
  display: flex;
  flex-direction: row;
}

.items {
  flex-flow: row wrap;
  justify-content: center;
  width: 500px;
  border-top: 1px solid black;
  border-bottom: 1px solid black;
}

h3 {
  align-items: center;
  justify-content: center;
  width: 250px;
  padding-right: 30px;
}

p {
  justify-content: space-between;
  padding: 0 5px;

}

.wrapper {
  justify-content: center;
}

</style>
