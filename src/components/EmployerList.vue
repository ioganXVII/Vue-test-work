<template>
    <div class="list">
    <ul>
      <li class="employer" v-for="employer in employers" :key = "employer.id">
          First Name: {{employer.first_name}} <br>
          Last Name: {{employer.last_name}} <br>
          Email: {{employer.email}} <br>
          Gender: {{employer.gender}} <br>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'EmployerList',
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
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
