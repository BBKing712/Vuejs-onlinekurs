<template>
  <div id="app">
    
  {{Name}},
  {{Alter}},
  {{Geschlecht}}
  <br>
  {{'${Name}'}}
  <br>
  {{Alter*2}}
  </div>
</template>

<script>


export default {
  name: 'App',
  data: () =>
  ({
    Name: 'Bernhard',
    Alter: 52,
    Geschlecht: 'männlich'

  })

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
