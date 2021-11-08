<template>
    <div class="list">
    <ul v-for="employer in employers" :key="employer.id">
          <ListElement :employer="employer"/>
    </ul>
  </div>
</template>

<script>
import ListElement from './ListElement.vue'

export default {
  name: 'EmployerList',
  components: {
    ListElement,
  },
  props: {
    employers: {
      type: Array,
      required: true,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  text-align: start;
  display: flex;
  justify-content: center;
  text-justify: 5px;
  list-style-type: none;
}

</style>
