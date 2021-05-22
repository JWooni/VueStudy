<template>
  <!-- <button @click="add">
    ADD
  </button> -->
  <!-- <h1 @click="changeMessage">
    {{ msg }}
  </h1> -->
  <!-- <h1>{{ reversedMessage }}</h1> -->
  <!-- <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1> -->
  <h1
    :class="{active:isActive}"
    @click="activate">
    Hello?!({{ isActive }})
  </h1>
</template>

<script>
export default {
  data(){
    return{
      // Getter, Setter
      //msg: 'Hello Computed!'
      // msg: 'Hello?'
      isActive: false
}
  },
  //computed:{
    // Getter
    // reversedMessage(){
    //   return this.msg.split('').reverse().join('')
    //  }
    // Getter, Setter
    // reversedMessage: {
    //   get(){
    //     return this.msg.split('').reverse().join('')
    //   },
    //   set(value){
    //     this.msg = value
    //   }
    // }
  //},
  // watch:{
  //   msg(newValue){
  //     console.log('msg:', newValue)
  //   },
  //   reversedMessage(newValue){
  //     console.log('reversedMessage', newValue)
  //   }
  // },
  methods: {
    // add(){
    //   this.reversedMessage += '!?'
    //   //this.msg += '?!'
    // }
    // changeMessage(){
    //   this.msg = 'Good!'
    // }
    activate(){
      this.isActive = true
    }
  }
}
</script>

<style scoped>
  .active{
    color: red;
    font-weight: bold;
  }
</style>