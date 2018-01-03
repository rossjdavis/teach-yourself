<template>
  <div class="wrapper">
    <h3>Education</h3>
    <div class="loc" v-for="loc in locs">
      <div class="loc-year"> {{ loc.year }} </div>
      <div class="loc-info">
        <div class="loc-head"> {{ loc.head }} </div>
        <div class="loc-name"> {{ loc.name }} </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Education',
  data() {
    return {
      locs: [
        {
          name: 'General Assembly',
          year: '2017-2018',
          head: 'WDI 19 Immersive Student'
        },
        {
          name: 'Jamestown Community College',
          year: '2007-2009',
          head: 'A.S., Computer Science'
        },
        {
          name: 'Erie Community College',
          year: '2013',
          head: 'A.S., Computer Science'
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

.loc {
  flex-direction: row;
  padding-top: 20px;
}

.loc:first-of-type {
  padding-top: 0px;
}

.loc-year {
  width: 250px;
  margin-right: 15px;
}

.loc-info {
  width: 500px;
  flex-direction: column;
}

.loc-head {
  font-weight: 500;
}

.loc-name {
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
