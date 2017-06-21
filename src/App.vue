<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view></router-view>
    <p v-on:click="addTest">
      {{test}}
    </p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data:function() {
    return{
      test:"test1"
    },
    methods: {
      addTest:function{
        console.log(this.test)
      }
    }
}
}
</script>
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
