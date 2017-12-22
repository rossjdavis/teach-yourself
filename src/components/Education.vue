<template>
  <div class="section">
    <h3>Education</h3>
    <div class="items">
      <p v-for="item in items">
        {{ item.item }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Education',
  data() {
    return {
      items: [
        { item: 'General Assembly, WDI 19 Student, 2017-2018' },
        {
          item: 'Jamestown Community College, A.S., Computer Science, 2007-2009'
        },
        { item: 'Erie Community College, A.S., Computer Science, 2013' }
      ]
    }
  }
}
</script>

<style scoped>
.section {
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
