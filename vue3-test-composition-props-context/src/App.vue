<template>
  <MyBtn
    class="jwooni"
    style="color: red;"
    @hello="log">
    Apple
  </MyBtn>
</template>

<script>
import MyBtn from '~/components/MyBtn'

export default {
  components: {
    MyBtn
  },
  methods: {
    log() {
      console.log('Hello world!')
    }
  }
}
</script>