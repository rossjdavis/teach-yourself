<template>
  <div class="wrapper">
    <h3>Experience</h3>
    <div class="job" v-for="job in jobs">
      <div class="job-year"> {{ job.year }} </div>
      <div class="job-info">
        <div class="job-head"> {{ job.head }} </div>
        <div class="job-name"> {{ job.name }} </div>
        <div class="job-role" v-for="role in job.role">
          <li> {{ role }} </li>
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
          city: 'Washington, D.C.',
          year: '2017-2018',
          head: 'Junior Developer Student',
          role: ['Web Developer Immersive', 'UX Design Bootcamp']
        },
        {
          name: 'Association of American Medical Colleges',
          city: 'Washington, D.C.',
          year: '2014',
          head: 'Help Desk Engineer',
          role: [
            'Decommissioned outdated systems and prepared new workstations for use.',
            'Assisted with the migration of IT infrastructure to the new office location.'
          ]
        },
        {
          name: 'Ingram Micro',
          city: 'Buffalo, N.Y.',
          year: '2010-2012',
          head: 'Technical Sales Consultant',
          role: [
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

div {
  display: flex;
  flex-direction: column;
}

.job {
  flex-direction: row;
  padding-top: 20px;
}

.job:first-of-type {
  padding-top: 0;
}

.job-year {
  width: 250px;
  margin-right: 15px;
}

.job-info {
  width: 500px;
  flex-direction: column;
}

.job-head {
  font-weight: 500;
}

.job-name {
  font-style: italic;
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
