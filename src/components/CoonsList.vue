<template>
  <ul>
    <li v-for="coon in coons">
      <!-- move it to external component -->
      <div id="coon">
        <div>
          {{ coon.id }}
        </div>
        <div>
          {{ coon.name }}
        </div>
        <div>
          {{ coon.state }}
        </div>
        <div>
          {{ coon.creator }}
        </div>
        <div>
          {{ coon.deadline }}
        </div>
      </div>
    </li>
  </ul>
</template>

<script>
  export default {
    name: 'coonsList',
    data () {
      return {
        coons: [
          {
            id: 1,
            name: 'new coon',
            state: 'new',
            creator: 'anp',
            description: {
              what: 'initiatives',
              why: 'because',
              how: 'code'
            },
            karma: 0,
            deadline: '2017-12-26'
          },
          {
            id: 2,
            name: 'new coon',
            state: 'new',
            creator: 'anp',
            description: {
              what: 'initiatives',
              why: 'because',
              how: 'code'
            },
            karma: 0,
            deadline: '2017-12-26'
          }
        ]
      }
    }
  }
</script>

<style scoped>
  #coon {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
</style>
