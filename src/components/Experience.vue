<template>
  <div class="xp">
    <h3>Experience</h3>
    <div class="job-list">
      <div class="job" v-for="job in jobs">
          {{job.name}}
          {{job.city}}
          {{job.year}}
          {{job.title}}
          <div v-for="role in job.roles">
            <span>{{role}}</span>
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
          name: 'AAMC',
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
.xp {
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  margin: 0 auto;
}

.job-list {
  display: flex;
  flex-direction: column;
  width: 500px;
}

h3 {
  display: flex;
  align-items: center;
  width: 250px;
  justify-content: center;
  padding-right: 30px;
}


</style>
