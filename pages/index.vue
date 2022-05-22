<template>
  <div>
    <component :testfunction="testfunction" :test="test" :is="page" />
  </div>
</template>



<script>
export default {
  name: 'IndexPage',
  data() {
    return {
       page:"Sudoku",
      test: "page",
    }
  },
  methods: {
    testfunction() {
      alert("testfunction")
    }
  }
}
</script>
