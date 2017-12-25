<template>
  <div class="wrapper">
    <h3>Experience</h3>
    <div class="job-list">
      <div class="job" v-for="job in jobs">
        <div class="job-head">
          <span>{{job.name}}, {{job.city}}, {{job.year}}</span>
        </div>
        <span>{{job.title}}</span>
        <div class="job-role" v-for="role in job.roles">
          <li>{{role}}</li>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Experience',
  data() {
    return {
      jobs: [
        {
          name: 'General Assembly',
          city: 'Washington, DC',
          year: '2017-2018',
          title: 'Student',
          roles: ['Web Developer Immersive', 'UX Design Bootcamp']
        },
        {
          name: 'Association of American Medical Colleges',
          city: 'Washington, DC',
          year: '2014',
          title: 'Help Desk Engineer',
          roles: [
            'Decommissioned outdated systems and prepared new workstations for use.',
            'Assisted with the migration of IT infrastructure to the new office location.'
          ]
        },
        {
          name: 'Ingram Micro',
          city: 'Buffalo, NY',
          year: '2010-2012',
          title: 'Technical Sales Consultant',
          roles: [
            'Designed enterprise technology solutions to resolve infrastructure problems.',
            'Managed the relationship between vendors and technical support to execute training plans and boost product sales.'
          ]
        }
      ]
    }
  }
}
</script>

<style scoped>

div, h3, span {
  display: flex;
  flex-direction: row;
}

.job,
.job-list {
  flex-direction: column;
  width: 500px;
}

.job {
  padding-bottom: 20px;
}

.job-head {
}

.job-list {
  border-bottom: 1px solid black;
}

.job-role {
  justify-content: flex-start;
  margin-left: 20px;
}

h3 {
  align-items: center;
  justify-content: center;
  width: 250px;
  padding-right: 30px;
}

.wrapper {
  justify-content: center;
  padding-top: 20px;
}


</style>
