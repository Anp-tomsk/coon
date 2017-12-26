<template>
  <div>
    <div>
      <h2>Coon form</h2>
    </div>
    <div>
      <h3>Name</h3>
      <input v-model="coon.name">
    </div>
    <div>
      <h3>State</h3>
      <input v-model="coon.state">
    </div>
    <div>
      <h3>Creator</h3>
      <input v-model="coon.creator">
    </div>
    <div>
      <h3>Description</h3>
      <h4>What</h4>
      <textarea v-model="coon.description.what"/>
      <h4>Why</h4>
      <textarea v-model="coon.description.why"/>
      <h4>How</h4>
      <textarea v-model="coon.description.how"/>
    </div>
    <div>
      <h3>Karma</h3>
      <input v-model="coon.karma">
      <button>+</button>
      <button>-</button>
    </div>
    <div>
      <h3>Deadline</h3>
      <input type="date" v-model="coon.deadline"/>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'coonForm',
    data () {
      return {
        coon: {
          id: 1,
          name: 'default coon',
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
      }
    }
  }
</script>


<style scoped>

</style>
