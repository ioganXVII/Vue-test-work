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
.list{
  text-align: start;
  display: flex;
  justify-content: center;
  text-justify: 5px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  line-height: 1.5rem;
  padding: 15px;
  border: 1px solid #cacaca;
  margin: 5px;
}
</style>
