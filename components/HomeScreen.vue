<template>
<div>
  <p>HomeScreen {{test}}</p>

  <button @click="()=>{testfunction()}">test</button>
</div>
</template>

<script>
export default {
  name: "HomeScreen",
  props:{
    test:"test",
    testfunction:()=>{alert(nope)}
  }
}
</script>

<style scoped>

</style>
