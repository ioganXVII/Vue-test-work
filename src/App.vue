<template>
  <div id="app">
    <EmployerList :employers="employers"/>
  </div>
</template>

<script>
import data from '../MOCK_DATA.json'

import EmployerList from './components/EmployerList.vue'

export default {
  name: 'App',
  components: {
    EmployerList
  },
  data(){
    return{
      employers: data,
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
