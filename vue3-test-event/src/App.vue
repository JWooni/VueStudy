<template>
  <button @click="handler('hi', $event)">
    Click 1
  </button>
  <button @click="handler('what', $event)">
    Click 2
  </button>
  <button @click="handlerA(), handlerB()">
    Click me
  </button>
</template>

<script>
export default {
  methods:{
    handlerA(){
      console.log('A')
    },
    handlerB(){
      console.log('B')
    }    
  }
}
</script>