<template>
  <div class="wrapper">
    <h3>Education</h3>
    <div class="items">
      <span v-for="item in items">
        {{ item.item }}
      </span>
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
div {
  display: flex;
  flex-direction: row;
}

.items {
  flex-direction: column;
  justify-content: flex-start;
  width: 500px;
}

h3 {
  display: flex;
  align-items: center;
  width: 250px;
  justify-content: center;
  padding-right: 30px;
}

.wrapper {
  justify-content: center;
  padding-top: 20px;
}

</style>
