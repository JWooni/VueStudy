<template>
  <img
    alt="Vue logo"
    src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />

  <!-- v-if -->
  <button @click="handler">
    click me!
  </button>
  <h1 v-if="isShow">
    Hello?!
  </h1>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  //name: 'App',
  // components: {
  //   HelloWorld
  // }

  data(){
    return{
      isShow: true
    }
  },
  methods:{
    handler(){
      this.isShow = !this.isShow
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
