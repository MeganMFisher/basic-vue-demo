
<template>
  <div id="app">
    <input v-model='message'/>
    <!-- <input v-bind:value='message' v-on:input='handleChange'/>  -->
    <!-- v-on:input like onChange -->
    <!-- : is the same as doing v-bind: -->
    <!-- @input is the same as doing v-on:input -->
    <p>{{message}}</p>
  </div>
</template>

<script>
// You don't have to export anything out of your file unless you are using JavaScript 

export default {
  data() {
    return {
      message: "Hello World"
      //this is your state
    }
  },
  methods: {
    // handleChange(e) {
    //   this.message = e.target.value
    // }
  }
}
</script>

<style scoped> 
/* Will scope your css for you so you don't have to worry about duplicating styles on other components. You can also select the language you want like sass. lang='sass'*/
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
