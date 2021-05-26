<!--
<template>
  <a
    href="https://naver.com"
    target="_blank"
    @click.prevent.once="handler">
    NAVER
  </a>
</template>
-->

<template>
  <div
    class="parent"
    @wheel.passive="handler">
    <div class="child"></div>
  </div>
</template>

<script>
export default {
  // methods:{
  //   handlerA(event){
  //     console.log(event.target)
  //     console.log(event.currentTarget)
  //     console.log('A')
  //   },
  //   handlerB(){
  //     console.log('B')
  //   }
  // }
  methods:{
    handler(event){
      for(let i = 0; i < 10000; i +=1){
        console.log(event)
      }
    }
  }
}
</script>

<style scoped lang="scss">
  .parent {
    width: 200px;
    height: 100px;
    background-color: royalblue;
    margin: 10px;
    padding: 10px;
    overflow: auto;
    .child{
      width: 100px;
      height: 2000px;
      background-color: orange;
    }
  }
</style>