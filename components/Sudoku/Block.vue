<template>
  <div class="sudoku-block">
    <p>{{number}}{{name}}</p>
  </div>
</template>

<script>
export default {
  name: "Block",
  props: {
    number: {
      type: Number,
      required: true
    },
    name: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
