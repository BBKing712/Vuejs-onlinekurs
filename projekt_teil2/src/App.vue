<template>
  <div id="app">
    
  {{firstName}}  {{lastName}},{{Alter}},{{Geschlecht}}
  <br>
  
  <u>{{fullName}},{{Alter}},{{Geschlecht}}</u>
  <br>

  {{Alter*2}}
  <br>
  {{Math.random()}}
  <br>
  {{Alter> 18 ? "volljährig" : "nicht volljährig"}}
  </div>
</template>

<script>


export default {
  name: 'App',
  data: () =>
  ({
    firstName: 'Bernhard',
    lastName: "Korn",
    Alter: 52,
    Geschlecht: 'männlich'


  }),
  computed: {
    fullName() {
      return this.firstName + ' ' + this.lastName;

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
