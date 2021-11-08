<template>
  <li>
      First Name: {{ employer.first_name }} <br>
      Last Name: {{ employer.last_name }} <br>
      E-mail: {{ employer.email }} <br>
      Gender: {{ employer.gender }} <br>
  </li>
</template>

<script>
export default {
    name: 'ListElement',
    props: {
        employer:{
            type: Array,
            required: true,
        }
    },
}
</script>

<style>
li {
  width: 250px;
  line-height: 1.5rem;
  padding: 15px;
  border: 1px solid #cacaca;
  margin: 5px;
}
</style>